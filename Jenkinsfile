pipeline {
  agent any

  tools {
    maven "maven3"
	
  }
  stages {

    stage('Build') {
      steps {
        sh 'https://github.com/vishnuprasadk0123/hcl_project.git'
        sh 'clean install'

      }

    }


  }

}