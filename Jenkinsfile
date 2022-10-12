pipeline {
    agent any
    stages{
        stage("build"){
            steps{
                echo "Building the project"
            }
        }
        post{
            success{
                emailext attachLog: true, body: 'email from jenkins', subject: 'test email', to: 'ynareshbabu1991@gmail.com'
            }
        }
    }
}
