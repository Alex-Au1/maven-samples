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

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('verify') {
      steps {
        sh 'mvn verify'
      }
    }

    stage('clean') {
      steps {
        sh 'mvn clean'
      }
    }

  }
  tools {
    maven 'DHT_MVN'
    jdk 'DHT_SENSE'
  }
}