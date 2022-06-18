pipeline {
  agent any
  stages {
    stage('log tool version') {
      steps {
        sh 'mvn --version'
      }
    }

    stage('codecompile') {
      steps {
        bat 'compile'
      }
    }

    stage('codereview') {
      steps {
        bat 'pmd:pmd'
      }
    }

  }
}