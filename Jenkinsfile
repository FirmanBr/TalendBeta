pipeline {
	agent any
    
    stages {
        stage('Checkout Repository') {
            steps {
                checkout scm
            }
        }
        stage('Set up Java') {
            agent {
                label 'ubuntu' // Menggunakan agent Ubuntu
            }
        }
		        
    }	
}
