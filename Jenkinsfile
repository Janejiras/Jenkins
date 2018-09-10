pipeline {
  agent any
  stages {
    stage('Intializ') {
      steps {
        echo 'Test'
        echo 'Minimal Pipelines'
      }
    }
    stage('Generate report') {
      steps {
        sh 'tar -czf target/reports-${GIT_COMMIT:0:6}.tar.gz blog/blue-ocean-editor'
      }
    }
  }
}