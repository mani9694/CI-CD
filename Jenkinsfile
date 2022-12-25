pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh '${which composer} install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
