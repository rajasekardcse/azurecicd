pipeline {
	agent any
	tools {
		maven "Maven"
		}
	stages {
		stage('Build Maven') {
		steps{
			checkout([$class: 'GitSCM', branches: [[name:'*/master']], extensions:[], userRemoteConfigs:[[url: 'https://github.com/rajasekardcse/azurecicd.git']]])
			
			sh "mvn -Dmaven.test.failure.ignore=true clean package"
			
			}
		}
	}
}


