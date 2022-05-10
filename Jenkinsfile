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
          steps {
            echo 'added java 8'
          }
        }

      }
    }

  }
  environment {
    BIzz_Name = 'worker bee'
  }
}