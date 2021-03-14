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
	    git 'https://github.com/vishnuprasadk0123/hcl_project.git'
        bat "mvn -Dmaven.test.failure.ignore=true clean test"

      }

    }
    stage('Deploy') {
      steps {

        bat "ansible-playbook deployWARFile.yml"

      }

    }

  }

}