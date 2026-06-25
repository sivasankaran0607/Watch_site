pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Code fetched from GitHub'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building Kia Website Application'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p deployment
                cp watchpage.html deployment/
                echo "Deployment completed: kia.html copied to deployment folder"
                '''
            }
        }
    }
}
