pipeline {
    agent any

    stages {
        stage('Cloning repository') {
            steps {
                git 'https://github.com/faizan2ahmed/MLOPs_Faizan.git'
            }
        }
        
        stage('Installation of dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
    }
}
