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

                sudo cp watchpage.html /var/www/html/watchpage.html
                echo "Deployment completed: kia.html copied to deloyment folder"
                '''
            }
        }
    }
}
