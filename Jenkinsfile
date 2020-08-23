// DECLARATIVE //
pipeline {
    
    agent any
    stages {

        stage('Build') {
            steps {
                def localVar = 'Jenkins sample' // Can be double quote too
                /* Add additional data about the build */
                echo "Build no ${BUILD_ID}"//only double quote when refering to environmental variable"
                echo "Build proceed at the location : ${WORKSPACE}"
                bat 'javac test.java'
                bat 'java test'
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
