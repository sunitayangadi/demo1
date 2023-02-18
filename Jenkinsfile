pipeline {
    agent any
             stage ('build') {
	     steps {
		     sh 'mvn clean install'
           }				 
	   
	   }
	   stage ('test') {
	       steps {
	     	     junit 'target/surefire-reports/*.*xml'
		   }
	   }
	   
	}
}
	 
