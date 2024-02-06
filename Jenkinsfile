pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'print a plan for project'
      }
    }

    stage('code') {
      steps {
        echo 'print a code '
      }
    }

    stage('build') {
      steps {
        echo 'print build message'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'print test message'
          }
        }

        stage('release') {
          steps {
            echo 'print release message'
          }
        }

        stage('deploy') {
          steps {
            echo 'print deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'print operate'
          }
        }

      }
    }

  }
}