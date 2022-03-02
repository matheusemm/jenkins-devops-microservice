pipeline {
	// agent any
	agent {
		docker {
			// image 'maven:3.6.3'
			image 'node:13.8'
		}
	}

	stages {
		stage('Build') {
			steps {
				echo "Build"
				// sh "mvn --version"
				sh "node --version"
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
			echo "I'm awesome. I run always."
		}
		success {
			echo "I run when you are successful."
		}
		failure {
			echo "I run when you fail."
		}
	}	
}
