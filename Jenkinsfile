pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting StudentManager from GitHub'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analyzing StudentManager code'
            }
        }

        stage('Quality Gate') {
            steps {
                echo 'Checking code quality'
            }
        }

    }
}