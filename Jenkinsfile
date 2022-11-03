pipeline {
    agent any
    stages {
        stage ('ok') {
            steps {
                echo 'ok'
            }
        }
    }
    post {
        always {
            emailext attachLog: true, body: 'test mail from jenkins', subject: 'Test Mail', to: 'ynareshbabu1991@gmail.com'
        }
    }
}
