pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello this build stage'
      }
    }

    stage('Test ') {
      parallel {
        stage('unit testing') {
          steps {
            echo 'testing '
            sh 'echo unit testing'
          }
        }

        stage('Test2') {
          steps {
            echo 'testing done'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'done'
      }
    }

  }
}