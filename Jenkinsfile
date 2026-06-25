pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Code pulled from GitHub!'
                sh 'java --version'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling Java code...'
                sh 'javac src/Main.java'
            }
        }
        stage('Run') {
            steps {
                echo 'Running the program...'
                sh 'java -cp src Main'
            }
        }
    }
}