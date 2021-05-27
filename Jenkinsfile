#!groovy

pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                //bat "git clone https://github.com/amritsingh0870/java_project.git"
                //bat "cd java_project"
                bat "javac App.java"
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
