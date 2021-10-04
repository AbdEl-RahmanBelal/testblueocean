pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Tests') {
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
        input(message: 'Are you sure to deploy?', ok: 'yes, I am sure')
        echo 'Deploy Completed'
      }
    }

    stage('notify for new build') {
      steps {
        echo 'new build completed'
      }
    }

  }
}