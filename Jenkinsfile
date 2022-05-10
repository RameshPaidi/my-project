pipeline {
  agent none
  stages {
    stage('Buzz Build') {
      agent {
        node {
          label 'java7'
        }

      }
      steps {
        echo 'added pipline'
      }
    }

  }
  environment {
    BIzz_Name = 'worker bee'
  }
}