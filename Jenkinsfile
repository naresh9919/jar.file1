pipeline{
    agent any
    tools {
        maven 'maven 3.8.6'
    }
    stages{
        stage('build maven'){
            steps{
                sh 'mvn clean install'
            }
        }
        stage('Build notification'){
            post{
                success{
                    mail to:"ynareshbabu1991@gmail.com", subject:"SUCCESS: ${currentBuild.fullDisplayName}", body: "Yay, we passed."
                }
                failure{
                    mail to:"ynareshbabu1991@gmail.com", subject:"FAILURE: ${currentBuild.fullDisplayName}", body: "Boo, we failed."
                }
            }
        }
    }
}
