pipeline {
    agent any
    stages {


        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'pytest test-main.py'
            }
        }

        stage('Run App') {
            steps {
                bat 'python main.py'
            }
        }
    }
}
