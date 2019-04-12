pipeline {
	agent none
	stages {
		stage('build') {
			agent { docker { image 'maven:3.3.3' } }
			steps {
				sh 'mvn --version'
			}
		}
		stage('Build') {
			agent any
			steps {
				sh 'echo "Hello World"'
				sh '''
					 echo "Multiline shell steps works too"
					 ls -lah
					 '''
			}
		}
	}
}
