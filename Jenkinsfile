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

        stage('Check Ubuntu Version') {
            steps {
                // Mengeksekusi perintah untuk memeriksa versi Ubuntu
                script {
                    sh 'lsb_release -a'
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
