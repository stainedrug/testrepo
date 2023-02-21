@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("Build Dockerfile"){
            steps {
                buildDockerFile()
            }
        }
        stage("Stage 2"){
            steps{
                echo "Stage 2"
               // script{
                    echo vcCredentials.usernameVariable
                    echo vcCredentials.credentialsId
               // }
            }
        }
        stage("stage 3"){
            steps{
                echo "Stage 3"
            }
        }
        stage("stage 4"){
            steps{
                echo "Stage 4"
            }
        }

    }
}
