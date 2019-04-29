pipeline {
    agent any

    environment {
        TAG = "${env.BUILD_NUMBER}"
    }

    stages {
        stage("Build") {
            steps {
                //ToDo: add code
            }
        }
        stage("docker") {
            steps {
                //ToDo: add code
            }
        }

        stage("deploy") {
            steps {
                script {
                    //ToDo: add code
                }

            }
        }
    }

    post {
        cleanup {
            deleteDir()
        }
    }
}