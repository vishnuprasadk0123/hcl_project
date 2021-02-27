pipeline {
  agent any

  tools {
    maven "maven3"
	
  }
  stages {

    stage('Build') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'mvn clean complie'

      }

    }

    stage('Test') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'mvn clean test'

      }

    }
    stage('Deploy') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'deployWARFile.yml'

      }

    }

  }

}