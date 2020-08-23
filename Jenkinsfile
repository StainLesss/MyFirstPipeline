// DECLARATIVE //
pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                echo 'Building..'

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

// SCRIPTED //
node {
    stage("Build"){
        echo '... building ...'
    }
    stage ('Test'){
        echo '... testing ...'
    }
    stage('Deploy'){
        echo '... deploy...'
    }
}
