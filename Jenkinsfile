pipeline {
  agent any
  stages {
    stage('Package') {
      steps {
        sh ''mvn -B -DskipTests -Dmaven.javadoc.skip=true clean package'
      }
    }
  }
}
