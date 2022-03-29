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
        stage('Release') {
            steps {
                echo 'Releasing the code.'
            }
        }
        post {
             always {
                 emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
             }
        }
    }
}
