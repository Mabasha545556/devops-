pipeline {
    agent Node-1
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
        stage ("webhook stage"){
            steps{
            echo 'welocme to webhooks'
            }
        }
    }
}
        
