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
                script {
                    def scannerHome = tool 'SonarScanner'

                    withSonarQubeEnv('SonarQubeServer') {
                        bat "\"${scannerHome}\\bin\\sonar-scanner.bat\""
                    }
                }
            }
        }

        stage('Quality Gate') {
            steps {
                echo 'Quality Gate will be configured next'
            }
        }

    }
}