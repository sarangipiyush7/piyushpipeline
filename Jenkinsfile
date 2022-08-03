pipeline {
  agent any
  stages {
    stage('Run & command') {
      steps {
        sh '''ls
pwd
date
cal 1998'''
      }
    }

    stage('Build') {
      steps {
        echo 'my name is piyush'
      }
    }

    stage('Deploy on test') {
      parallel {
        stage('Deploy on test') {
          steps {
            echo 'deploy on test'
          }
        }

        stage('echo par') {
          steps {
            echo 'parallely build'
          }
        }

      }
    }

    stage('Deploy on prod') {
      steps {
        echo 'love jenkins'
        sleep 3
      }
    }

  }
}