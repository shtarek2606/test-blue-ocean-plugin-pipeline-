pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed ....'
      }
    }

    stage('test stages') {
      parallel {
        stage('test 1') {
          steps {
            echo 'running test1'
          }
        }

        stage('test2') {
          steps {
            echo 'running test 2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed'
      }
    }

  }
}