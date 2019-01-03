pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Compile') {
          steps {
            echo 'CleanCompile'
          }
        }
        stage('Build') {
          steps {
            echo 'Building Project files..'
          }
        }
      }
    }
    stage('Test') {
      parallel {
        stage('Test-Firefox') {
          steps {
            echo 'FirefoxTesting..;exit 1'
          }
        }
        stage('Test-IE') {
          steps {
            echo 'IETesting'
          }
        }
        stage('Test-Chrome') {
          steps {
            echo 'Testing-Chrome..'
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
  environment {
    Envrnment = 'XDev'
  }
}
