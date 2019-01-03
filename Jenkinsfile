pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }
    stage('Test') {
      parallel {
        stage('Test Firefox') {
          steps {
            echo 'TF'
          }
        }
        stage('Test Chrome') {
          steps {
            echo 'TC'
          }
        }
        stage('Test Edge') {
          steps {
            echo 'te; exit'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }
  }
}
