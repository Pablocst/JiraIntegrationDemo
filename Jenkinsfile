pipeline {
        agent any
        stages {
            stage('Build') {
                steps {
                    // Your build steps here
                    sh 'echo "Building..."'
                    // Send build information to Jira
                    jiraSendBuildInfo()
                }
            }
            stage('Deploy') {
                steps {
                    // Your deployment steps here
                    sh 'echo "Deploying..."'
                    // Send deployment information to Jira
                    jiraSendDeploymentInfo()
                }
            }
        }
    }
