pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Récupère le code depuis le dépôt GitHub
                git branch: 'main', url: 'https://github.com/Mohamed23012/Devops.git'
            }
        }
        stage('Compile') {
            steps {
                script {
                    // Compile le code Java
                    sh 'javac HelloWorld.java'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    // Exécute le code Java compilé
                    sh 'java HelloWorld'
                }
            }
        }
    }
}
