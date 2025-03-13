pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG22CS473 main.cpp'
            }
        }
        
        stage('Test') {
            steps {
                sh 'exit 1' //Error command
                //sh './PES2UG22CS473'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
