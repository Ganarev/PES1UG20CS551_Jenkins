pipeline {
	    agent any
	

	    stages {
	        stage('Build') {
	            steps {
	                sh 'g++ PES1UG20CS551.cpp -o PES1UG20CS551'
	                 build job: 'PES1UG20CS551-1', wait: false
	                 echo 'Build by CS551 successful'
	            }
	        }
	

	        stage('Test') {
	            steps {
	                sh 'cat PES1UG20CS551.cpp'
	                echo 'Test by CS551 successful'
	            }
	        }
	

	        stage('Deploy') {
	            steps {
	               
	                echo 'Deploy by CS551 successful'
	            }
	        }
	    }
	

	    post {
	        failure {
	            
	                echo 'Pipeline Failed'
	          
	        }
	    }
	}
