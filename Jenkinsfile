pipeline {
	agent { docker { image 'node:17.6'} }
	stages {
		stage('Build') {
			steps {
				sh "node --version"
				echo "Build"
			}
			
		}
		stage('Test') {
			steps {
				echo "Test"
			}
			
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
			
		}
	}
	post {
		always {
			echo "I'm awesome. I run always"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "I run when you are failed"
		}
	}
}
	
