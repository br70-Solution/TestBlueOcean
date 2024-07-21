pipeline {
  agent any
  stages {
    stage('Built') {
      steps {
        echo 'Built stage complete'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test1 complete'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2 Complete'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Complete'
      }
    }

  }
}