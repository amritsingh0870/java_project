#!groovy

pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                sh "mvn -version"
                sh "mvn clean install"
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
