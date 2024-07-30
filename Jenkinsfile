@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("run cxone scan"){
           steps{
            sh "echo 'Downloading CxOne CLI v${csEnvironment.cxVersion}'"
            //sh "wget -O ./cxcli.tar.gz 'https://github.com/Checkmarx/ast-cli/releases/download/${CX_VERSION}/ast-cli_${CX_VERSION}_linux_x64.tar.gz'"
            //sh "tar xzvf ./cxcli.tar.gz"
           }
        }
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
