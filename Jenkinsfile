pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo sh java -version
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo sh docker --version
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
