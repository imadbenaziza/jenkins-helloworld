pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "This is the build stage"'
            }
        } 

        stage('Approval') { 
            steps {
                input {
                    message 'Do you approve this?'
                    ok 'Yes'
                }
            }
        }

        stage('Test') {
            steps {
                sh 'echo "This is the test stage"'
            }
        }
    }
}


