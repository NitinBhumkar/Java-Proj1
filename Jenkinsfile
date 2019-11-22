pipeline {
	agent{label 'Master'}
	stages {
	stage ("SCM Checkout"){
		steps {
			   git 'https://github.com/NitinBhumkar/Java-Proj1.git'
			  }
		}
	stage ("Java execute"){
		steps {
			   sh label: '', script: 'javac *.java java Simple'
			  }
		}
	}	
}
