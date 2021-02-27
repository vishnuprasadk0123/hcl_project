pipeline {
  agent any

  tools {
    maven "maven3"

  }
  stages {

    stage('Compile') {
      steps {
        bat "clean complie"

      }

    }

    stage('Test') {
      steps {
        bat "clean test"

      }

    }
    stage('Deploy') {
      steps {

        bat "deployWARFile.yml"

      }

    }

  }

}