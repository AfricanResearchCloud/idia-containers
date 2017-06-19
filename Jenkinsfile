pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'This is the start of the pipeline'
      }
    }
    stage('Build') {
      steps {
        sh 'make all '
      }
    }
  }
}