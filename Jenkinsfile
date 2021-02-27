pipeline {
  agent any

  tools {
    maven "M2_HOME"
	
  }
  stages {

    stage('Build') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'mvn -Dmaven.test.failure.ignore=true clean complie'

      }

    }

    stage('Test') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'mvn -Dmaven.test.failure.ignore=true clean test'

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