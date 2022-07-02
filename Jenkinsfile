pipeline {
  agent any
  stages {
    stage('ansible') {
      parallel {
        stage('ansible') {
          steps {
            sh 'echo andible'
          }
        }

        stage('other') {
          steps {
            sh 'echo other'
          }
        }

      }
    }

    stage('finish') {
      steps {
        sh 'echo done'
      }
    }

  }
}