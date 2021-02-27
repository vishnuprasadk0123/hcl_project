pipeline {
  agent any

  tools {
    maven "maven3"

  }
  stages {

    stage('Build') {
      steps {
	  
	    git 'https://github.com/vishnuprasadk0123/hcl_project.git'
        bat "mvn -Dmaven.test.failure.ignore=true clean package"

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