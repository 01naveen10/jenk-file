pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // No need to execute npm install and npm run build if it's already done in the Dockerfile
            }
        }
        stage('Deploy') {
            steps {
                script {
                    def image = docker.image('01naveen10/simple-nodejs-website:latest')  // Reference the existing Docker image
                    image.run('-p 3000:3000')  // Run the Docker container with port mapping
                }
            }
        }
    }
}
