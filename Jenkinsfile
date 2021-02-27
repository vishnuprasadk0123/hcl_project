pipeline {
	agent any
	stage{
			
				stage('Checkout') {
					steps {
						checkout scm			        }
				}
			
				stage('Build') {
					steps {
					    sh 'M2_HOME'
						sh 'mvn clean build'
				 
						}
		
				}
				stage('deploy') {
					steps {
						sh 'deployWARFile.yml'
				 
						}
		
				}

			
			
			}
		
	}

