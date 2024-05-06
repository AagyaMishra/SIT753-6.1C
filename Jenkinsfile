pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Building the code ..."
                // Add commands to build the code using your build automation tool (e.g., Maven)
            }
            post {
                success {
                    // Send email notification on successful build
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Build Status",
                        body: "Build was successful.",
                    )
                }
                failure {
                    // Send email notification on failed build
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Build Status",
                        body: "Build failed. Please check the logs for details.",
                    )
                }
            }
        }
        
        stage("Unit and Integration Tests") {
            steps {
                echo "Running unit and integration tests ..."
                // Add your test commands here
            }
            post {
                success {
                    // Send email notification on successful test execution
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Unit and Integration Tests Status",
                        body: "Unit and Integration Tests were successful.",
                    )
                }
            }
        }
        
        stage("Code Analysis") {
            steps {
                echo "Performing code analysis ..."
                // Add commands to run your code analysis tool (e.g., SonarQube)
            }
            post {
                success {
                    // Send email notification on successful code analysis
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Code Analysis Status",
                        body: "Code analysis was successful.",
                    )
                }
            }
        }
        
        stage("Security Scan") {
            steps {
                echo "Performing security scan ..."
                // Add commands to run your security scanning tool (e.g., OWASP ZAP)
            }
            post {
                success {
                    // Send email notification on successful security scan
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Security Scan Status",
                        body: "Security scan was successful.",
                    )
                }
            }
        }
        
        stage("Deploy to Staging") {
            steps {
                echo "Deploying to staging server ..."
                // Add commands to deploy to staging server (e.g., AWS EC2)
            }
            post {
                success {
                    // Send email notification on successful deployment to staging
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Deploy to Staging Status",
                        body: "Deployment to staging server was successful.",
                    )
                }
            }
        }
        
        stage("Integration Tests on Staging") {
            steps {
                echo "Running integration tests on staging ..."
                // Add commands to run integration tests on staging environment
            }
            post {
                success {
                    // Send email notification on successful integration tests on staging
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Integration Tests on Staging Status",
                        body: "Integration tests on staging were successful.",
                    )
                }
            }
        }
        
        stage("Deploy to Production") {
            steps {
                echo "Deploying to production server ..."
                // Add commands to deploy to production server (e.g., AWS EC2)
            }
            post {
                success {
                    // Send email notification on successful deployment to production
                    emailext (
                        to: "aagyamishra403@gmail.com",
                        subject: "Deploy to Production Status",
                        body: "Deployment to production server was successful.",
                    )
                }
            }
        }
    }
}
