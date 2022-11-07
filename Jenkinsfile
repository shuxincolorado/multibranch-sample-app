pipeline {
  agent any //{label 'linux'}
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
    stage('Build') {
      steps {
        //sh './gradlew clean check --no-daemon'
        echo 'Hello world inside Jenkinsfile'
      }
    }
  }
}