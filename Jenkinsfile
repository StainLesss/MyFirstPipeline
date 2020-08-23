// DECLARATIVE //
pipeline {
    
    
    
    agent any
    stages {

        stage('Build') {
            steps {
                 input message: 'Please provide a input', parameters: [string(defaultValue: '', description: '', name: 'UserInputParameter', trim: false)]
               
                echo "User entered the value : ${params.UserInputParameter}"            
                echo "Build no ${BUILD_ID}"//only double quote when refering to environmental variable"
                echo "Build proceed at the location : ${WORKSPACE}"
                echo pwd()  // pwd show the current location and deleteDir() remove recursivly the files
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
                sleep 10  // Sleep 10 seconde
                /*  sleep time: 10, unit: 'NANOSECONDS'   can be change with NANOSECONDS / MICROSECONDS / MICROSECONDS / MINUTES / HOURS / DAYS */
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
