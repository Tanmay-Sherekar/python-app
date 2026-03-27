pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/your-username/python-jenkins-app.git'
            }
        }

        stage('Check Python') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Run App') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest'
            }
        }
    }
}
