pipeline{
    agent {
        label 'node1'
    }
    
    stages {
        stage ("build number and current login username") {
            steps{
                echo "the build number is ${BUILD_NUMBER} and current login username is ${USER}"
            }
        }
        stage ("email"){
           steps{
               sh 'echo "${var_email}"
           } 
        }
    }
}
