pipeline {
		agent {
			docker {
				alwaysPull true
				image 'maven:3.9.6'
			}
		}
		stages {
			stage('Build') {
                steps {
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
				echo "Im awesome. I run always"
			}
			success {
				echo "I run when you are successful"
			}
			failure {
				echo "I run when you are fail"
			}
		}

}

