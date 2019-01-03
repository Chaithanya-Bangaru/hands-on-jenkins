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
            echo 'TF; Exit /B 2'
          }
        }
        stage('Test Chrome') {
          steps {
            echo 'TC'
          }
        }
        stage('Test Edge') {
          steps {
            echo 'te'
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
