pipeline {
  agent any
  stages {
    stage('package') {
      steps {
        sh 'mvn clean package'
      }
    }
    stage('in server') {
      steps {
        sh 'cd xxl-sso-server/target/'
      }
    }
    stage('start') {
      steps {
        sh 'java -jar xxl-sso-server-0.1.1-SNAPSHOT.jar'
      }
    }
  }
}