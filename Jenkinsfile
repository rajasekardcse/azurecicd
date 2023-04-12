pipeline {
	agent any
	environment {
		PATH = "C:\Users\rajas\Documents\Learnings.config\Maven.config\apache-maven-3.9.0\bin:$PATH"
	}
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
