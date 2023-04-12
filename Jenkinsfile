pipeline {
	agent any
	tools {
		maven 'MAVEN'
		}
	stages {
		stage('Build Maven') {
		steps{
			echo 'Hello world'
			checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/rajasekardcse/azurecicd.git']])
			
			sh "mvn -Dmaven.test.failure.ignore=true clean package"
			
			}
		}
	}
}


