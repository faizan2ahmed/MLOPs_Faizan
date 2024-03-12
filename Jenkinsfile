pipeline {
    agent any

    stages {
        stage('Cloning repository') {
            steps {
                git branch: 'main', url: 'https://github.com/faizan2ahmed/MLOPs_Faizan.git'
            }
        }
        
        stage('Installation of dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Execution of test.py') {
            steps {
                bat 'python test.py'
            }
        }
    }
}
