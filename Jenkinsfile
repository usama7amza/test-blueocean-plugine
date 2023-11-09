pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test is done'
            sleep 1
          }
        }

        stage('test 2') {
          steps {
            echo 'test 2 id done'
          }
        }

      }
    }

    stage('build') {
      steps {
        echo 'build '
      }
    }

    stage('deploy') {
      steps {
        echo 'dep'
        fileExists 'jenkinsfile'
      }
    }

  }
}