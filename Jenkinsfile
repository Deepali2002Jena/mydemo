pipeline {
    agent any
	environment { 
        shyam= 'redhat'
    }

    stages {
        stage('run my custom variable') {
            steps {
				sh 'echo $shyam'
				sh 'date'
            }
        }
		
    }
