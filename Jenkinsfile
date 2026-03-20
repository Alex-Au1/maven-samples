pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/Alex-Au1/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}