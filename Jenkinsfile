pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello this build stage'
      }
    }

    stage('Test') {
      steps {
        build 'first job'
        sh 'echo "Here the job is built in blue ocean"'
      }
    }

    stage('deploy') {
      steps {
        echo 'deployment stage'
      }
    }

  }
}