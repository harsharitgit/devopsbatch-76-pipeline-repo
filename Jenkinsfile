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
      steps {
        echo 'I had to build on CI/CD'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'I had a test to work on CI/CD'
          }
        }

        stage('release') {
          steps {
            echo 'I had to release the work of CI/CD'
          }
        }

        stage('deploy') {
          steps {
            echo 'i had deployed ci/cd'
          }
        }

        stage('operate') {
          steps {
            echo 'operate /cicd'
          }
        }

      }
    }

  }
}