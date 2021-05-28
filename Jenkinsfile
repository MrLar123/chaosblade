pipeline {
  agent any
  stages {
    stage('chaos_alpha') {
      parallel {
        stage('chaos_alpha') {
          steps {
            echo 'Alpha'
          }
        }

        stage('view_code') {
          steps {
            sh '''ls -l
pwd'''
            timestamps()
          }
        }

        stage('deploy') {
          steps {
            input 'waite'
          }
        }

      }
    }

  }
}