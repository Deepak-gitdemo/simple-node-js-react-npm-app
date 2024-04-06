pipeline {
    agent any
    tools{ nodejs 'node'
    }
    stages {
        stage('Pre-Build') { 
            steps {
                sh 'npm install'
		sh 'npm --version'
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
