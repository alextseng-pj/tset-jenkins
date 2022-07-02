pipeline {
  agent any
  stages {
    stage('git') {
      parallel {
        stage('git pull') {
          steps {
            sh 'echo "git pull"'
          }
        }

        stage('other') {
          steps {
            sh 'echo "other"'
          }
        }

      }
    }

    stage('update conf.d') {
      steps {
        sh 'echo "ansible update conf.d"'
      }
    }

    stage('finish') {
      steps {
        sh 'echo "done"'
      }
    }

  }
}