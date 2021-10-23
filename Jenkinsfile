pipeline {
    agent {lable 'Node-1':'Node-2'}
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
        
