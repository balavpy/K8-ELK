pipeline {
agent any 
stages {
		stage ('promotheus') {
			steps {
				sh 'kubectl apply -f promotheus.yaml'
			}
		}
		stage ('logstash') {
			steps {
				sh 'kubectl apply -f logstash.yaml'
			}
		}
	}
}
