pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Teats') {
      parallel {
        stage('test1') {
          steps {
            echo 'test1 completed'
          }
        }

        stage('test2') {
          steps {
            echo 'test2 completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Completed'
      }
    }

  }
}