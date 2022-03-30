pipeline {
    agent any
    
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the code'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the Code'
          }
        }
        stage('Test') {
            steps {
                echo 'Testing the Code'
     }
 }
        stage('Release approval'){
            steps {
             input "Deploy to prod?"
         }
        }
        stage('Production') {
            steps {
                echo 'Releasing the code to production.'
            }
        } 
    }
}
