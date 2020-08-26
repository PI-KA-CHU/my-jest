pipeline {
    agent any
    
    stages { 
        stage('Pre-Process') { 
            steps {
                bat 'npm install --registry=https://registry.npm.taobao.org'
            }
        }

        stage('Build') {
            steps {
                echo 'start build'
                bat 'npm run build'
            }
        }

        stage('Test') {
            steps {
                echo 'start Test'
                bat 'npm run test'
            }
        }
    }
}
