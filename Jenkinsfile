pipeline {
    agent any
    environment {
        SERVICE_CREDS = credentials('mypass')
        }
		stages{
		   stage('Load credential'){
            steps {
                sh 'echo $SERVICE_CREDS_USR'
                sh 'echo $SERVICE_CREDS_PSW'
            }
		}
	}
}
