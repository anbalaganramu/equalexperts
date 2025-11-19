pipeline {
    agent any
    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/anbalaganramu/equalexperts.git'
            }
        }
        stage('Build a docker image') {
            steps {
                   sh "docker build -t experts ."            
            }
        }
    }
}
