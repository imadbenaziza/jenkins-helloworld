pipeline {
    agent any

    stages {
        // Stage for building
        stage('Build') {
            steps {
                // Print a message indicating the build stage
                sh 'echo "This is the build stage"'
            }
        }

        // Stage for manual approval
        stage('Approval') {
            steps {
                // Requesting user input for approval
                input {
                    message 'Do you approve this?'
                    ok 'Yes'
                }
            }
        }

        // Stage for testing
        stage('Test') {
            steps {
                // Print a message indicating the test stage
                sh 'echo "This is the test stage"'
            }
        }
    }
}

