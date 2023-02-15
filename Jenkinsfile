
//Declarative
pipeline {
	agent { docker { image 'maven:3.6.3'} }
	stages {
		stage('Build') {
			steps{
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps{
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps{
				echo "IntTest"
			}
		}	
	} 
	
	post {
		always {
			echo "I'm awesome. I run always"
		}
		success {
			echo "I run only when you are successful!"
		}
		failure {
			echo "I run only when you are fail!"
		}
	}
}
