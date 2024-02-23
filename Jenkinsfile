pipeline {
    agent {
        docker { image 'trainwithshubham/django-app:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'django-admin --version'
            }
        }
    }
}
