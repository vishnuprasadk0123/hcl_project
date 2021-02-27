pipeline {
  agent any

  stages {

    stage('Build') {
      steps {
        sh "maven3"
        sh "mvn clean install"

      }

    }

  }

}