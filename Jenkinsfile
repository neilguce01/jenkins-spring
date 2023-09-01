pipeline {
  agent any
  tools { maven 'M3' }
  stages {
    stage('Build') {
      steps {
        bat 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        bat 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        bat 'mvn package'
      }
    }
  }
}
