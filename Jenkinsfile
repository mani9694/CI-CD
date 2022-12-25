pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'composer:latest'
                }
            }
            steps {
                // Download dependencies
                sh "composer install --ignore-platform-reqs --no-scripts --no-dev --no-interaction --no-progress"
                
                // Dump the autoloader (for performance)
                sh "composer dump-autoload --optimize --no-interaction"
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
