pipeline {
    agent {
        docker { 
            image 'trainwithshubham/django-app:latest'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Deploy') {
            steps {
                sh 'django-admin --version'
            }
        }
    }
}
