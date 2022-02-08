pipeline {
  agent any
  stages {
    stage('App 1') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "Karan is great"'
          }
        }

        stage('Test 1') {
          steps {
            sh 'echo "I am good"'
          }
        }

      }
    }

    stage('App - 2') {
      parallel {
        stage('Build-2') {
          steps {
            sh 'echo "Souarv is great"'
          }
        }

        stage('Test -2') {
          steps {
            sh 'echo sai > test.log'
          }
        }

      }
    }

    stage('Archive') {
      steps {
        archiveArtifacts '*.log'
      }
    }

  }
}