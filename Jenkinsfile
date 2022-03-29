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
                timeout(time: 1, unit: 'MINUTES') {
                    retry(5) {
                echo 'Deploying the Code
               }
            }
          }
        }
        stage('Test') {
            steps {
                echo 'Testing the Code'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing the code.'
            }
        }     
    }
}
