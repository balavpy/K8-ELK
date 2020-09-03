pipeline {
agent any 
stages {
		stage ('promotheus') {
			steps {
				sh 'kubectl apply -f promotheus.yaml'
				sh 'sleep 80'
			}
		}
		stage ('logstash') {
			steps {
				sh 'kubectl apply -f logstash.yaml'
				sh 'sleep 60'
			}
		}
		stage ('filebeat') {
			steps {
				sh 'kubectl apply -f filebeat.yaml'
				sh 'sleep 60'
			}
		}
		stage ('kibana') {
			steps {
				sh 'kubectl apply -f kibana.yaml'
				sh 'sleep 60'
			}
		}
	}
}
