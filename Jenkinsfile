@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("CredentialCheck"){
           // environment{
              //creds1 = credentials('security-API-user')
              //creds2 = credentials('security_API_user')
          //  }
            steps {
                echo "Stage 1"
                //sh 'printenv'
            }
        }
        stage("Stage 2"){
            steps{
                echo "Stage 2"
               // script{
                    //echo vcCredentials.usernameVariable
                    //echo vcCredentials.credentialsId
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
