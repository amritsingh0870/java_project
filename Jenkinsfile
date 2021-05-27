#!groovy

pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                bat "java App"
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
