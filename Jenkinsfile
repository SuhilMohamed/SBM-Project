pipeline {
  agent any
  stages {
    stage('Build APP') {
      steps {
        echo 'Start Building'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Frontend') {
          steps {
            echo 'Testing The Frontend'
          }
        }

        stage('Test Backend') {
          steps {
            echo 'Testing The Backend'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying Success'
      }
    }

  }
}