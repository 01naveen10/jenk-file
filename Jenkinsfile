pipeline {
    agent {
        docker { image '01naveen10/simple-nodejs-website:latest' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'node server.js'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker run -d -p 3000:3000 01naveen10/simple-nodejs-website:latest'
            }
        }
    }
}
