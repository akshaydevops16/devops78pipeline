pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'I want to plan my application development'
      }
    }

    stage('Code') {
      steps {
        echo 'development team perform the app development'
      }
    }

    stage('Build') {
      steps {
        echo 'build the application'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing team performing the testing activity'
          }
        }

        stage('Deploy') {
          steps {
            echo 'deploy the war files'
          }
        }

        stage('Release') {
          steps {
            echo 'move to release'
          }
        }

        stage('Operate') {
          steps {
            echo 'test application functionality'
          }
        }

      }
    }

  }
}