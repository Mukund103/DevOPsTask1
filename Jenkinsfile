pipeline {
  agent any
  stages {
    stage('Buid1') {
      parallel {
        stage('Buid1') {
          agent any
          steps {
            git(url: 'https://github.com/Mukund103/DevOPsTask1.git', branch: 'main', changelog: true)
            cleanWs(cleanWhenSuccess: true)
          }
        }

        stage('Build2') {
          steps {
            echo '"Build2"'
          }
        }

      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo '"Build1 successful"'
          }
        }

        stage('Test2') {
          steps {
            sh 'echo \'Build2 successfull\''
          }
        }

      }
    }

  }
}