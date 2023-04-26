pipeline{
    agent {
        label 'node1'
    }
    
    stages {
        stage ("build number and current login username") {
            steps{
                sh 'echo "the build number is ${BUILD_NUMBER} and current login username is ${USER}" > /home/node1/aishwarya/file1.txt '
            }
        }
        stage ("email"){
           steps{
               sh 'echo "${var_email}" >> /home/node1/aishwarya/file1.txt'
           } 
        }
    }
}
