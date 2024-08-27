pipeline {
	agent any
	parameters {
  choice choices: ['DEV', 'QA', 'UAT'], name: 'Environment'
}

	stages {
	    stage('Checkout') {
	        steps {
		      git 'https://github.com/siddhipande3/BAKU.git'			       
				}
		stage('Build') {
	           steps {
			  sh 'mvn install'
	                 }
		stage('Deployment'){
		    steps {
			script {
			 if (env.ENVIRONMENT == 'QA' ){
        	sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps

        	echo "deployment has been done on QA!"
			 }
			else if ( env.ENVIRONMENT} == 'UAT' ){
    		sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps'
    		echo "deployment has been done on UAT!"
			}
			
			}}}	
} } 
