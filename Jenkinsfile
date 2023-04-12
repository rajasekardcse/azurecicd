pipeline {
	agent any
	tools {
		maven "Maven"
		}
	stages {
		stage('Build Maven') {
		steps{
			git "https://github.com/rajasekardcse/azurecicd.git", 
			
			sh "mvn -Dmaven.test.failure.ignore=true clean package"
			
			}
		}
	}
}


