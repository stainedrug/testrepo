@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("CredentialCheck"){
            environment{
              creds1 = credentials('security-API-user')
              creds2 = credentials('security_API_user')
            }
            steps {
                sh 'printenv'
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
          //  agent {
          //      docker {
          //          image 'node:16.13.1-alpine'
         //       }
         //  }
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
