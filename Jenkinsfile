pipeline {
    agent any

    stages {
        stage("Github Setup"){
            steps {
            git credentialsId: 'github', url: 'https://github.com/arslan578/jenkins_app.git'
            }
        }
        stage("A"){

            steps{
       
                echo "====++++executing A++++===="
            }
            post{
                always{
                    echo "====++++always++++===="
                }
                success{
                    echo "====++++A executed successfully++++===="
                }
                failure{
                    echo "====++++A execution failed++++===="
                }
        
            }
        }
    }
        
}
