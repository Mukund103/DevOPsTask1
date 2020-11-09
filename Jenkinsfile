pipeline {
  agent any
  stages {
    stage('Buid1') {
      parallel {
        stage('Buid1') {
          steps {
            git(url: 'https://github.com/Mukund103/DevOPsTask1.git', branch: 'main', changelog: true)
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
      steps {
        echo '"Build1 successful"'
      }
    }

  }
}