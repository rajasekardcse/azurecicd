pipeline {
	agent any
	stages {
		stage('clone code')
		{
		steps{
			git credentialsId: 'git_credentials', url: 'https://github.com/rajasekardcse/azurecicd.git'
			}
		}
		stage('build') 
		{
		steps{
			sh "mvn clean install"
			}
		}
	}
}
