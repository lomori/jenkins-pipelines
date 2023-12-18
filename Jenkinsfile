pipeline {
  agent {
    kubernetes {
      //cloud 'kubernetes'
      containerTemplate {
        name 'node'
        image 'node:20.10.0-alpine3.19'
        command 'sleep'
        args '99d'
      }
    }
  }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
