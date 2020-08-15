pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh java -version
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh docker --version
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
