pipeline {
    agent any
    environment {
        SERVICE_CREDS = credentials('mypass')
        }
		stages{
            steps {
                sh 'echo "Service user is $ SERVICE_CREDS_USR"'
                sh 'echo "Service password is $ SERVICE_CREDS_PSW"'
            }
		}
	}
}
