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
    }
}
