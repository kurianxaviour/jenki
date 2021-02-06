pipeline {
	agent any
	tools {
    	maven 'M3'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/judy-simplilearn/Calculator.git'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	}
    	}
	}
}
