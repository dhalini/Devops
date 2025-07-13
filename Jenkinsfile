pipeline {
    agent any
    stages {


        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest test_main.py'
            }
        }

        stage('Run App') {
            steps {
                sh 'python main.py'
            }
        }
    }
}
