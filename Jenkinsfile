pipeline {
    agent any
    
    stages{
        stage('Build'){
            steps{
                echo "Building application"
            }
        }
        
        stage('Test'){
            steps{
                echo 'Testing application'
            }
        }
        
        stage('Deploy'){
            steps{
                echo "Deploying application"
            }
        }
    }
    
    post{
        always{
            emailext body: 'Summary', subject: 'pipeline status', to: 'sagnikskb0nyp437@gmail.com'
        }
    }
}
