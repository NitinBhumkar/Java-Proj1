pipeline {
	agent{label 'Master'}
	options {
  buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '1', numToKeepStr: '1')
}
	stages {
	   stage ("Header"){
			steps {
			echo 'Hello ! SCM pipeline script on Github is executing now!!'
		        }
	         }	
		
	   stage ("Announce"){
			steps {
			echo 'Hello ! Fetching Java Content from GitHUB!!'
		        }
	         }
	
	   stage ("SCM Checkout"){
			steps {
			   git 'https://github.com/NitinBhumkar/Java-Proj1.git'
			  }
		}
		
	   stage ("Announce1"){
			steps {
			echo 'Hello This is beginning of Java script!!'
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
		           echo 'Hello!!  SCM pipeline script completed'
			}
		}
	}
}
