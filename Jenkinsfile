pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is first stage'
          }
        }

        stage('build2') {
          steps {
            sh 'ls'
          }
        }

      }
    }

    stage('CQ') {
      steps {
        sh 'pwd'
      }
    }

    stage('deploy_SIT') {
      steps {
        sleep 5
      }
    }

    stage('deploy_to_UAT') {
      steps {
        echo 'this is final satge'
      }
    }

  }
}