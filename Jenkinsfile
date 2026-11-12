
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Recuperation du projet Java depuis GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Compilation du projet avec Maven'
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Execution des tests'
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                echo 'Creation du fichier JAR'
                sh 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Development'
            }
        }
    }
}
