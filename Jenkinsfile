pipeline {
	agent any
	stages {
		stage('Git') {
			steps {
				git 'https://github.com/JavierCGI/JenkinsPruebas.git'
			}
		}
		stage('Build') {
			steps {
				sh 'javac HolaMundo.java'
			}
		}
		stage('Test') {
			steps {
				sh 'java HolaMundo'
			}
		}
	}
}
