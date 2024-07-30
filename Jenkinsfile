@Library('mygithub') _
pipeline {
    agent any
    stages {
        stage("run cxone scan"){
            steps{
                withCredentials ([usernamePassword(credentialsId: 'APIUSERNAME', usernameVariable: 'security_user', passwordVariable: 'security_pass')]){
                    sh '''
                        echo $security_user 
                        echo $security_pass
                        '''                    
                 }
                sh "echo 'Downloading CxOne CLI v${csEnvironment.cxVersion}'"
                sh "wget -O ./cxcli.tar.gz 'https://github.com/Checkmarx/ast-cli/releases/download/${csEnvironment.cxVersion}/ast-cli_${csEnvironment.cxVersion}_linux_x64.tar.gz'"
                sh "tar xzvf ./cxcli.tar.gz"
            //sh """
            //    ./cx scan create -s ${env.WORKSPACE} \
            //    --project-name "${env.JOB_NAME}" \
            //    --branch "${env.BRANCH_NAME}" \
            //    --agent 'Jenkins' \
            //    --base-uri "${CX_BASE_URI}" \
            //    --tenant "${CX_TENANT}" \
            //    --client-id "${CX_CLIENT_ID}" \
            //    --client-secret "${CX_CLIENT_SECRET}" \
            //    --scan-types "sast,iac-security,sca,api-security" \
            //    --report-format pdf \
            //    --report-pdf-email luis-vicente.soto-salinas@dxc.com \
            //    --wait-delay 60
            //"""
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
