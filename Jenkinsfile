pipeline {
    agent any
    stages{
        stage ("Git Checkout"){
            steps{
            git 'https://github.com/Mabasha545556/devops-.git'
            }
        }
        stage ("Maven Build"){
            steps{
            sh 'mvn clean install package'
            }
        } 
        stage ("Test stage"){
            steps{
            echo 'welocme to devops'
            }
        }
        stage ("webhook stage"){
            steps{
            echo 'welocme to webhooks'
            }
        }
    }
}
        
