pipeline {
  agent any
  stages {
    stage('package') {
      steps {
        sh 'mvn clean package'
      }
    }
    stage('start') {
      steps {
        sh 'java -jar xxl-sso-server/target/xxl-sso-server-0.1.1-SNAPSHOT.jar'
      }
    }
  }
}