pipeline {
	agent any
	parameters {
  choice choices: ['DEV', 'QA', 'UAT'], name: 'Environment'
}

	stages {
	    stage('Checkout') {
	        steps {
<<<<<<< HEAD
		      git 'https://github.com/siddhipande3/BAKU.git'			       
				}
=======
		      git  'https://github.com/siddhipande3/BAKU.git'			       
				}}
>>>>>>> ebe5f24366b9e7e662490c6de728523b3bfb0e38
		stage('Build') {
	           steps {
			  sh 'mvn install'
	                 }
		stage('Deployment'){
		    steps {
			script {
			 if (env.ENVIRONMENT == 'QA' ){
<<<<<<< HEAD
        	sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps

        	echo "deployment has been done on QA!"
			 }
			else if ( env.ENVIRONMENT} == 'UAT' ){
    		sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps'
    		echo "deployment has been done on UAT!"
			}
			
			}}}	
} } 
=======
        	sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps'

        	echo "deployment has been done on QA!"
			 }
			else if ( env.ENVIRONMENT == 'UAT' ){
    		sh 'cp target/BAKU.war /home/siddhi/Downloads/apache-tomcat-9.0.93/webapps'
    		echo "deployment has been done on UAT!"
			
			}}}	
} }
	} }
>>>>>>> ebe5f24366b9e7e662490c6de728523b3bfb0e38
