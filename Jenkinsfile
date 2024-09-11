pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the Git repository
                git url: 'https://github.com/abhaybisht9412/Jenkins-test.git', credentialsId: '951f8b4c-b5c4-4f9a-b1b8-2fc156389b71'
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
  
