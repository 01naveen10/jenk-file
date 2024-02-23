pipeline {
    agent any
    
    stages {
        stage('Deploy') {
            steps {
                script {
                    docker {
                        image '01naveen10/simple-nodejs-website:latest'  // Reference the existing Docker image
                        args '-p 3000:3000'  // Port mapping option
                    }
                }
            }
        }
    }
}
