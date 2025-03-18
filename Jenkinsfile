
pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building the project...'
                    sh 'g++ -o PES1UG22CS504-1 WRONG.cpp' 
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    echo 'Testing the project...'
                    sh './PES1UG22CS504-1' 
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying the project...'
                    sh 'echo Deployment successful' 
                }
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
