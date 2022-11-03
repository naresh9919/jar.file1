pipeline{
    agent any
    stages{
        stage("buildin"){
            steps{
                echo "building the project"
            }
        }
        post{
            success{
                emailext body: 'email sent out from the jenkins', subject: 'Test Email', to: 'ynareshbabu1991@gmail.com'
            }
        }
    }
}
