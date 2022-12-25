pipeline {
    agent any
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stages {
            stage('Test') {
                steps {
                    sh 'node --version'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
