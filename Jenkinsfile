pipeline {
    agent any
	environment { 
        shyam= 'redhat'
    }
	parameters { 
	 string(name: "person", defaultValue: "Deepali Jena", description: "how are babes")
	 choice(name: "mychoice", choices: "debug\nrelease", description: "choose build type")
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
        stage('check your choice') {
            steps {
				sh 'echo $mychoice'
				
            }
        }
		stage('Example') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
			}
			steps{
			  echo "plz run this code"
			}
		}
    }
}
