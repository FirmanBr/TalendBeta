pipeline {
	agent any
    
    stages {
	
        stage('Setup') {
            steps {
                // Menggunakan Windows sebagai agent
                script {
                    // Membuat label 'windows' untuk agent Windows
                    agent { label 'windows' }
                }
            }
        }

        stage('Check Windows Version') {
            steps {
                // Mengeksekusi perintah untuk memeriksa versi Windows
                script {
                    // Menggunakan perintah untuk menampilkan versi Windows
                    bat 'ver'
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
