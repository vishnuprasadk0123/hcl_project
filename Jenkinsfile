pipeline {
  agent any

  tools {
    maven "maven3"

  }
  stages {

    stage('Compile') {
      steps {
        bat "mvn clean complie"

      }

    }

    stage('Test') {
      steps {
        bat "mvn clean test"

      }

    }
    stage('Deploy') {
      steps {

        bat "deployWARFile.yml"

      }

    }

  }

}