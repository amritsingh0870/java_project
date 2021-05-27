#!groovy

pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                sh "java App"
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
