pipeline {
	agent any
	stages {
		stage("Build") {
			steps {
				sh 'echo "Building..."'
				sh 'chmod +x build.sh'
				sh './build.sh'
			}
		}
		stage("Test") {
			steps {
				sh 'echo "Makinf file..."'
				sh 'make'
			}
		}
		stage("Deploy") {
			steps {
				sh 'echo "Deploying file..."'
				sh './jenkins-test-2'
			}
		}	
	}
}
