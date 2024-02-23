pipeline {
    agent {
        docker { 
            image '01naveen10/simple-nodejs-website:latest'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Deploy') {
            steps {
                sh 'node server.js'
            }
        }
    }
}
