@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("CredentialCheck"){
            steps {
                echo csCredentials.credentialsId
                echo csCredentials.usernameVariable
                echo csCredentials.passwordVariable
            }
        }
        stage("Stage 2"){
            steps{
                echo "Stage 2"
                    script{
                        echo csCredentials.credentialsId
                        echo csCredentials.usernameVariable
                        echo csCredentials.passwordVariable
                    }
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
