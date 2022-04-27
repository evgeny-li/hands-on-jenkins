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
            bat 'echo \'Testing Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            bat 'echo \'Testing Chrome\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}