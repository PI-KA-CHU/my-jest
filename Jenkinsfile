pipeline {
    agent any
    
    environment {
        CI = 'true'
    }
    
    stages { 
        stage('Pre-Process') { 
            steps {
                bat 'npm install --registry=https://registry.npm.taobao.org'
            }
        }

        stage('Test') {
            steps {
                echo 'start Test'
                bat 'npm run test'
            }
        }
        
        stage('Build') {
            steps {
                echo 'start build'
                bat 'npm run build'
            }
        }
        
    }
}
