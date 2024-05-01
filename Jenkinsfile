pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Define build steps here
            }
        }
        stage('Test') {
            steps {
                // Define test steps here
            }
        }
        stage('Deploy') {
            steps {
                // Define deployment steps here
            }
        }
        // post {
    success {
        emailext body: "Pipeline execution successful",
                 subject: "Pipeline Status: Success",
                 to: "aagyamishra403@email.com"
    }
    failure {
        emailext body: "Pipeline execution failed",
                 subject: "Pipeline Status: Failure",
                 to: "aagyamishra403@email.com"
    }
    always {
        emailext body: "Test and security scan stages completed",
                 subject: "Pipeline Stage Status",
                 to: "aagyamishra403@email.com"
    }
}

    

