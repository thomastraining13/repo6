pipeline {
  agent any
  stages {
    stage('') {
      steps {
        echo 'hi build'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('integration') {
          steps {
            echo 'integrration testing'
          }
        }

        stage('unit testing') {
          steps {
            echo 'unit testing'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}