pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }
    stage('Test Firefox') {
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
            echo 'te; EXIT /B 4'
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
