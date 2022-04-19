pipeline {
	agent any
	tools {
		maven 'MAVEN385'
		jdk 'JAVA11JDK'
	}
	
	stages {
	
		stage('Compile Stage') {
			steps {
				sh 'mvn clean compile'
			}
		}	
		
		stage('Testing Stage') {
			steps {
				sh 'mvn test'	
			}
		}	
		
			
		stage('Verify Stage') {
			steps {
					sh 'mvn verify'
			}
		}
	}
}