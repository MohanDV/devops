pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building.......'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            echo 'Testinf Firefox'
          }
        }

        stage('Test Chrome') {
          steps {
            echo 'Testing Chrome '
            sh 'exit 1'
          }
        }

        stage('Test Edge') {
          steps {
            echo 'Testing edge '
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}
