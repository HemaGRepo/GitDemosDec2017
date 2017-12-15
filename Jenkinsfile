pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Success'
      }
    }
    stage('G1') {
      parallel {
        stage('Testing') {
          steps {
            echo 'Test 1 successfule'
          }
        }
        stage('Test1') {
          steps {
            echo 'Test 2 Success'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }
  }
}