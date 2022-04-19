pipeline {
	agent any
	
	stages {
		stage('Compile Stage') {
		
			steps {
				withMaven(maven : 'MAVEN385') {
					sh 'mvn clean compile'
				}	
			}
		}	
		
		
		stage('Testing Stage') {
		
			steps {
				withMaven(maven : 'MAVEN385') {
					sh 'mvn test'
				}	
			}
		}	
		
			
		stage('Verify Stage') {
		
			steps {
				withMaven(maven : 'MAVEN385') {
					sh 'mvn verify'
				}	
			}
		}
	}
}