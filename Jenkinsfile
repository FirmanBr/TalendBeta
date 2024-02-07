pipeline {
	agent any
    
    stages {
	
        stage('Setup') {
            steps {
                // Menggunakan Ubuntu sebagai agent
                script {
                    // Membuat label 'ubuntu' untuk agent Ubuntu
                    agent { label 'ubuntu' }
                }
            }
		}	
			
        stage('Checkout Repository') {
            steps {
                checkout scm
            }
        }

		        
    }	
}
