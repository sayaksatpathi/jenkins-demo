pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Repository cloned successfully'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Testing Application...'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploying Application...'
            }
        }
    }
}
