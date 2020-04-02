pipeline{
	agent any 
	tools{
		maven 'LocalMaven'
		jdk 'jdk-12.0.1'
	}
	stages{
		stage('--clean--'){
			steps{
				bat 'mvn clean'
			}
		}

		stage('--test--'){
			steps{
				bat 'mvn test'
			}
		}

		stage('--package--'){
			steps{
				bat 'mvn package'
			}
		}
	}
}
