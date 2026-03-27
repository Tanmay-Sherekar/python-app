pipeline {
    agent any

    stages {

        stage('Clone GitHub Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/Tanmay-Sherekar/python-app.git'
            }
        }

        stage('Check Python Version') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run Python App') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
