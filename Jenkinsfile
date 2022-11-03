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
                mail to:"ynareshbabu1991@gmail.com", subject:"SUCCESS: ${currentBuild.fullDisplayName}", body: "Yay, we passed."
            }
        }
    }
}
