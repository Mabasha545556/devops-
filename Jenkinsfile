pipeline {
    agent any
    stages{
        stage ("Git Checkout"){
            steps{
                git 'https://github.com/Mabasha545556/devops-.git', branch: "${params.branch}"
            }
        }
        stage ("Maven Build"){
            steps{
            sh 'mvn clean install package'
            }
        } 
        stage ("Parameter stage"){
            steps{
            properties([parameters([choice(choices: 'dev\ntest\nprod', description: 'select branch for build', name: 'stages')])])
            }
        }
        stage ("webhook stage"){
            steps{
            echo 'welocme to webhooks'
            }
        }
    }
}
        
