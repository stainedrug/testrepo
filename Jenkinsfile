@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("CredentialCheck"){
            steps {
                echo vcCredentials.credentialsId
                echo vcCredentials.usernameVariable
                echo vcCredentials.passwordVariable
            }
        }
        stage("Stage 2"){
            steps{
                echo "Stage 2"
                    script{
                        echo vcCredentials.credentialsId
                        echo vcCredentials.usernameVariable
                        echo vcCredentials.passwordVariable
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
