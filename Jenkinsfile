pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test Successfully'
          }
        }

        stage('error') {
          steps {
            echo 'Test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy Successfully'
        sleep 30
      }
    }

  }
}