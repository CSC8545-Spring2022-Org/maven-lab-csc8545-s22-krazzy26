pipeline {
	agent any
	tools {
		maven 'MAVEN385'
		jdk 'JAVA11JDK'
	}
	
	stages {
	
		stage('Compile Stage') {
			steps {
				bat 'mvn clean compile'
			}
		}	
		
		stage('Testing Stage') {
			steps {
				bat 'mvn test'	
			}
		}	
		
			
		stage('Verify Stage') {
			steps {
					bat 'mvn verify'
			}
		}
	}
}
