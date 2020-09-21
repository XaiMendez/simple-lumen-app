pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building...'
          }
        }

        stage('') {
          steps {
            readTrusted 'https://github.com/XaiMendez/pipeline-build-lumen-app/blob/master/Jenkinsfile'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }

  }
}