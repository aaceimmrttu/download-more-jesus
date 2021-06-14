pipeline {
    agent any
    stages {
        stage('Lint') {
            agent {
                docker {
                    image 'node:latest'
                    args '-p 3000:3000'
                }
            }
            steps {
                sh 'npm run lint'
            }
        }
        stage('Build') {
            agent { label "docker"}
            steps {
                script {
                     def imageId = docker.build("rollforbugs/download-more-jesus:${env.BUILD_ID}")
                     echo "Built: ${imageId}"
                     //imageId.push()
                }
            }
        }
    }
}