pipeline {
    agent any
	environment { 
        shyam= 'redhat'
    }
	parameters { 
	 string(name: "person", defaultValue: "Deepali Jena", description: "how are babes")
	 choice(name: "mychoice", choices: "debug/nrelerase", description: "choose build type")
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
        stage('run my choice parametrised') {
            steps {
				sh 'echo $mychoice'
				
            }
        }
    }
}
