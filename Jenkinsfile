pipeline {
    agent any
    environment {
	    region = "us-east-1"
        docker_repo_uri = "136954245697.dkr.ecr.us-east-1.amazonaws.com/upgrad-assignment"
		task_def_arn = ""
        cluster = ""
        exec_role_arn = ""
    }
    stages {
        stage('Example') {
            steps {
                echo 'This is a sample stage'
            }
        }
	stage('Build') {
            steps {
                docker.build("upgrad-assignment")
            }
        }
    }
}