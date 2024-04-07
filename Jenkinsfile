pipeline {
    agent any
    tools{ nodejs 'node'
    }
    stages {
        stage('Pre-Build') { 
            steps {
                bat 'npm install'
		bat 'npm --version'
            }
        }

        stage('Build') {
            steps {
                bat 'npm run build'
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
