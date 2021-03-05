pipeline {
  agent any
  stages {
    stage('Devel') {
      steps {
        echo 'This is dev stage'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Branch1'
          }
        }

        stage('Build2') {
          steps {
            echo 'Build2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy stage'
      }
    }

  }
}