pipeline {
    agent any

    environment {
        TAG = "${env.BUILD_NUMBER}"
    }

    stages {
        stage("Build") {
            steps {
                withMaven("maven"){
                    sh "mvn clean package"
                }
            }
        }
        /*
        stage("docker") {
            steps {
                //ToDo: add code
            }
        }
        */
        /*
        stage("deploy") {
            steps {
                script {
                    //ToDo: add code
                }

            }
        }
        */
    }

    post {
        cleanup {
            deleteDir()
        }
    }
}