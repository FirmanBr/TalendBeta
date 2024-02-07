pipeline {
	agent any
    
    stages {
        stage('Checkout Repository') {
            steps {
                checkout scm
            }
        }
		
        stage('Run Talend Job') {
            steps {
                sh './TalendLinux/TalendTesting/TalendTesting_run.sh'
            }
        }        
    }	
}
