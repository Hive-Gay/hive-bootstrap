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
          sh "npm run scss"
        }
      }
    }

    stage('Upload') {
      steps {
        script {
          sh "mc cp dest/hive-bootstrap.css hive/cdn/hive-bootstrap-${BRANCH_NAME}.css"
        }
      }
    }
  }
}
