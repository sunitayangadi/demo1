pipeline {
    agent any
             stage ('build') {
	     steps {
		     sh 'mvn clean package'
           }				 
	   
	   }
	   stage ('test') {
	       steps {
	     	     junit 'target/surefire-reports/*.*xml'
		   }
	   }
	   
	}
}
	 
