pipeline {
agent any 
stages {
		stage ('promotheus') {
			steps {
				sh 'kubectl apply -f promotheus.yaml'
			}
		}
	}
}
