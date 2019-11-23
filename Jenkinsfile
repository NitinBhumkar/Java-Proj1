pipeline {
	agent{label 'Master'}
	stages {
	stage ("cleanup"){
		steps {
			cleanWs()
buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '1', numToKeepStr: '1')
		}
	}			
	stage ("SCM Checkout"){
		steps {
			   git 'https://github.com/NitinBhumkar/Java-Proj1.git'
			  }
		}
	stage ("Java execute"){
		steps {
			   sh label: '', script: '''javac *.java 
			   java Simple'''
			  }
			}
		stage ("Footer"){
			steps {
				echo 'Hello!! This is SCM pipeline script running from github'
			}
		{
	}	
}
