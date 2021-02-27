pipeline {
  agent any

  tools {
    maven "maven3"

  }
  stages {

    stage('Compile') {
      steps {
        sh "mvn clean complie"

      }

    }

    stage('Test') {
      steps {
        sh "mvn clean test"

      }

    }
    stage('Deploy') {
      steps {

        sh "deployWARFile.yml"

      }

    }

  }

}