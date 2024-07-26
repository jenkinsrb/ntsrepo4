pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM Stage Successful'
      }
    }

    stage('Deploy_Dev&QA') {
      parallel {
        stage('Deploy_Dev') {
          agent any
          steps {
            echo 'Dev Successful'
          }
        }

        stage('Deploy_QA') {
          agent any
          steps {
            echo 'QA Successful'
          }
        }

      }
    }

    stage('Deploy_Prod') {
      agent any
      steps {
        echo 'Prod Successful'
      }
    }

  }
}