//SCRIPTED
/* node {
	echo "Build"
	echo "Test"
	echo "Test"
} */

//DECLARATIVE
pipeline {
	agent any
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
			echo "i'm awesome. i always run"
		}
		success {
			echo "SUCCESS"
		}
		failure {
			echo "i'm failing"
		}
	}
}