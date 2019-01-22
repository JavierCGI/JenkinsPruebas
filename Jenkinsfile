pipeline {
  agent any
  stages {
    stage('prueba1y2') {
      parallel {
        stage('prueba1') {
          steps {
            sh 'echo "prueba1"'
          }
        }
        stage('prueba2') {
          steps {
            sh 'echo "prueba2"'
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'echo "prueba3"'
      }
    }
  }
}