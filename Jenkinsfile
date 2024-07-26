pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM Stage Successful'
      }
    }

    stage('Deploy_Dev') {
      parallel {
        stage('Deploy_Dev') {
          steps {
            echo 'Dev Successful'
          }
        }

        stage('Deploy_QA') {
          steps {
            echo 'QA Successful'
          }
        }

      }
    }

    stage('Deploy_Prod') {
      steps {
        echo 'Prod Successful'
      }
    }

  }
}