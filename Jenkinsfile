pipeline {
    agent any
	environment { 
        shyam= 'redhat'
    }
	parameters { 
	 string(name: "person", defaultValue: "Deepali Jena", description: "how are babes")
	 choice(name: "mychoice", choices: "debug\nrelease", description: "choose build type")
	 booleanParam(name: "DEBUG_BUILD", defaultValue: true, description: "enter true ya false")
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
		stage('check your boolean parameter') {
            steps {
				sh 'echo $DEBUG_BUILD'
				
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
