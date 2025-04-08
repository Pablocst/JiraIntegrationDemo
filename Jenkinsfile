pipeline {
        agent any
        stages {
            stage('Build') {
                steps {
                    // Your build steps here
                    sh 'echo "Building..."'
                    // Send build information to Jira
                    jiraSendBuildInfo(jiraSite: 'palbuquerque.atlassian.net', issueKey: 'DFM-2')
                }
            }
            stage('Deploy') {
                steps {
                    // Your deployment steps here
                    sh 'echo "Deploying..."'
                    // Send deployment information to Jira
                    jiraSendDeploymentInfo(jiraSite: 'palbuquerque.atlassian.net', issueKey: 'DFM-2')
                }
            }
        }
    }
