pipeline {
  agent none
  stages {
    stage('Buzz Build') {
      parallel {
        stage('Buzz Build') {
          steps {
            echo 'added pipline'
          }
        }

        stage('build7') {
          agent {
            node {
              label 'java7'
            }

          }
          steps {
            echo 'added java 7 node '
          }
        }

        stage('build 8') {
          agent {
            node {
              label 'java8'
            }

          }
          environment {
            BUZZ_NAME = 'java bees'
          }
          steps {
            echo 'added java 8'
            sh 'echo I am a $BUZZ_NAME!'
          }
        }

      }
    }

    stage('Buzz Test') {
      parallel {
        stage('Buzz Test') {
          steps {
            echo 'added buzz test stage'
          }
        }

        stage('Testing a') {
          steps {
            echo 'added testinga '
          }
        }

        stage('Testing b') {
          steps {
            echo 'addeed testing b'
          }
        }

      }
    }

  }
  environment {
    BIzz_Name = 'worker bee'
  }
}