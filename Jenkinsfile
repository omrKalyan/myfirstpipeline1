pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "This is first pipeline build in BlueOcean"'
          }
        }

        stage('test') {
          steps {
            sh 'echo "This is parallely happening in test Phase"'
          }
        }

      }
    }

    stage('UAT') {
      steps {
        sh 'echo "Test Completed"'
      }
    }

  }
}