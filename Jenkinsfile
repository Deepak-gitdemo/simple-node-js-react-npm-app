pipeline {
    agent any
    stages {
        stage('Pre-Build') { 
            steps {
                sh 'npm install' 
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Build successfully completed'
                echo 'Deploying the Code'
            }
        }
    }
}
