pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date
cal'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is my testing server '
          }
        }

        stage('') {
          steps {
            sh '''ls
ll'''
          }
        }

      }
    }

    stage('Deploy to Prod') {
      steps {
        sleep 15
      }
    }

  }
}