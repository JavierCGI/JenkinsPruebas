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
    stage('prueba3') {
      steps {
        sh 'echo "prueba3"'
      }
    }
    stage('PWD') {
      steps {
        pwd()
      }
    }
    stage('sleep 3') {
      steps {
        sleep 3
      }
    }
    stage('comprueba fichero') {
      steps {
        fileExists 'prueba'
      }
    }
    stage('escribir fichero') {
      steps {
        writeFile(file: 'pruebaescribir', text: 'pruebaescribir')
      }
    }
    stage('correo') {
      steps {
        mail(subject: 'pruebacorreo', body: 'pruebacorreo', to: 'javier.lopezgonzalez@cgi.com')
      }
    }
  }
}