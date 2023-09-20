pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'I have a plan to work on CI/CD'
      }
    }

    stage('code') {
      steps {
        echo 'I had a development where i worked on CI/CD'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'I had to build on CI/CD'
          }
        }

        stage('test') {
          steps {
            echo 'working on test ci/cd'
          }
        }

        stage('release') {
          steps {
            echo 'working on release ci/cd'
          }
        }

        stage('deploy') {
          steps {
            echo 'working on deployment ci/cd'
          }
        }

        stage('operate') {
          steps {
            echo 'working on operate ci/cd'
          }
        }

      }
    }

  }
}