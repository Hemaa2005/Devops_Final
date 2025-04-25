pipeline {
    agent any

    triggers {
    pollSCM('H/5 * * * *')  // Polls GitHub every 5 minutes
    }

    stages {
        stage('Clone Repository') {
            steps {
                git credentialsId: 'Github', url: 'https://github.com/Hemaa2005/Devops_Final.git', branch: 'main'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
