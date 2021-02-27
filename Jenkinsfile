pipeline {
	agent any

	tools {
		maven "M2_HOME"
	    			        
		    }
			stage{
				stage('Build') {
					steps {
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

