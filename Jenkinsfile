// DECLARATIVE //
pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                echo 'Building..'
                echo JENKINS_HOME
                echo WORKSPACE
                bat 'javac test.java'
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
