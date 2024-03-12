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
                        sh 'cat requirements.txt'
                        sh 'pip install --verbose -r requirements.txt'
                    }
                }
            }
        }
    }
}
