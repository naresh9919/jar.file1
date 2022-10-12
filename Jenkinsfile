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
                emailext body: 'test massage out from jenkins', subject: 'Test massage', to: 'ynareshbabu1991@gmail.com'
            }
        }
    }
}
