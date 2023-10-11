pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('Test') {
      steps {
        echo 'I want to test'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'I want to stage'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy'
          }
        }

        stage('Operate') {
          steps {
            echo 'I want to operate'
          }
        }

      }
    }

  }
}