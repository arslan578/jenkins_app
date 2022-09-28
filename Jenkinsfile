pipeline {
    agent any

    stages {
        stage("A"){
            steps{
                git 'https://github.com/arslan578/jenkins_app.git'
                echo "====++++executing A+++===="
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
