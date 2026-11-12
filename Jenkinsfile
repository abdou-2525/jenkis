
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Recuperation du projet Java'
            }
        }

        stage('Build') {
            steps {
                echo 'Compilation du projet avec Maven'
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Execution des tests'
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                echo 'Creation du fichier JAR'
                bat 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Development'
            }
        }
    }
}
