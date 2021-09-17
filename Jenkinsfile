pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello this build stage'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo "test the job"'
          }
        }

        stage('Test Done') {
          steps {
            echo 'test done'
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