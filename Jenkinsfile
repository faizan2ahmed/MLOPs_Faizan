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
                dir('MLOPs_Faizan') {
                    script {
                        bat 'type requirements.txt'
                        bat 'pip install --verbose -r requirements.txt'
                    }
                }
            }
        }
    }
}
