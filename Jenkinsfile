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
		
        stage('Execute Talend Testing') {
            steps {
                // Menjalankan file batch TalendTesting_run.bat
                script {
                    // Ganti path dengan lokasi aktual file batch
                    bat 'TalendTesting\\TalendTesting_run.bat'
                }
            }
        }		
		
        stage('Unit Test') {
            steps {
                echo 'Hello, Unit Test !'
            }
        }
        
        stage('Integration Test') {
            steps {
                echo 'Hello, Integration Test !'
            }
        }
        stage('Deployment') {
            steps {
                echo 'Hello, Deployment!'
            }
        }		
		        
    }	
}
