pipeline {
	agent any
    
    stages {
        stage('Checkout Repository') {
            steps {
                checkout scm
            }
        }
		
        stage('Set execute permission for TalendTesting_run.sh') {
            steps {
                dir('TalendLinux/TalendTesting') {
                    sh 'chmod +x TalendTesting_run.sh'
                }
            }
        }
        stage('Run Talend Job') {
            steps {
                sh './TalendLinux/TalendTesting/TalendTesting_run.sh'
            }
        }        
    }	
}
