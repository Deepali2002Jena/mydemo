pipeline {
    agent any
	environment { 
        shyam= 'redhat'
    }
	parameters { 
	 string(name: "person", defaultValue: 'Deepali Jena', description: 'how are babes')
	}

    stages {
        stage('run my custom variable') {
            steps {
				sh 'echo $shyam'
				sh 'date'
            }
        }
		stage('run my string parametrised') {
            steps {
				sh 'echo $person'
            }
        }
		
    }
}

