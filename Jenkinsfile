pipeline {
	    agent any
	

	    triggers {
	        pollSCM '* * * * *'
	    }
	    stages {
	        stage('Build') {
	            steps {
	                sh './gradlew build --no daemon'
	            }
	        }
	        stage('Test') {
	            steps {
	                sh './gradlew test'
	            }
	        }
	    }
	}
