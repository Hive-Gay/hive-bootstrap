pipeline {
  agent any;

  stages {

    stage('Setup') {
      steps {
        script {
          sh "npm install"
        }
      }
    }

    stage('Build') {
      steps {
        script {
          sh "npm scss"
        }
      }
    }
    
  }
}
