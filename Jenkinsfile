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
            echo 'TF; exit 0'
          }
        }
        stage('Test Chrome') {
          steps {
            echo 'TC'
          }
        }
        stage('Test Edge') {
          steps {
            echo 'te
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
