pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Hemaa2005/Devops_Final.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
