pipeline{
    agent any
    stages{
        stage('SCM Checkout'){
            steps{
                sh 'git credentialsId: 'BitbucketCreds', url: 'https://hari-vasunooru-selflearning@bitbucket.org/hari-vasunooru-selflearning/webapp-multibranch-pipeline.git''
            }
        }
        stage('Maven Build'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}