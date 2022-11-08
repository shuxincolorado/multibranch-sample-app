pipeline {
  agent any //{label 'linux'}
   
  //trigger for mid night every day
  triggers { 
    cron('0 0 * * *') 
  }

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

  post{
    always{
      echo "this should show up always no matter what."
    }
  }
}