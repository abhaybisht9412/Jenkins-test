pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the Git repository
                git url: 'https://github.com/abhaybisht9412/Jenkins-test.git'
            }
        }
        stage('Deploy') {
            steps {
                // Copy static files to the appropriate directory
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
