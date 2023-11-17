pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'I want to plan my application developemrnt'
      }
    }

    stage('code') {
      steps {
        echo 'Developement team perform the development of the application'
      }
    }

    stage('build') {
      steps {
        echo 'build the app'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing team test the activities'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the war files'
          }
        }

        stage('release') {
          steps {
            echo 'move to release'
          }
        }

        stage('operate') {
          steps {
            echo 'test the application'
          }
        }

      }
    }

  }
}