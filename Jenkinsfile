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
            build 'build-lumen-container'
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
  post {
    always {
      cleanWs()
    }
  }
}