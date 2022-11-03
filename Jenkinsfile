pipeline {
    agent any
    stages{
        stage("Buildin"){
            steps{
                echo "Building the project"
            }
        }
        post{
            success{
                emailext body: 'email sent out from the jenkins', subject: 'Test Email', to: 'ynareshbabu1991@gmail.com'
            }
        }
    }
}
