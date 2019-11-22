pipeline{
	agent{label 'Master'}
	stage ("SCM Checkout"){
		steps {
			   git 'https://github.com/NitinBhumkar/Java-Proj1.git'
			  }
			}
	stage ("Java executre"){
		steps {
			   sh label: '', script: 'javac *.java java Simple'
			  }
			}
		}
	}
