pipeline {
	agent any
	stages {
		stage ('build') {
			steps {
				sh 'mvn clean install'
			}
		
		}
		stage ('test') {
			steps {
		                 junit 'target/surefire-reports/*.*xml'
			         archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
			}
		}
	
	}
}
