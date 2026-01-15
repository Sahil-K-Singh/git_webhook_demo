pipeline {
    agent any
    stages {
        stage('hello') {
            steps {
               echo "pushed happened in repo"
            }
        }
    }
    post {
        success {
            mail to: 'singhsahil812003@gmail.com',
            subject: 'jenkins job triggered',
            body: "Y pushed happen in repo by sahil our jenkins mail was sucessful\n\nJob Name: ${env.JOB_NAME}\nBuild Number: ${env.BUILD_NUMBER}\nBuild URL: ${env.BUILD_URL}"
        }
    }
}
