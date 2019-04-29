pipeline {
    agent any

    environment {
        TAG = "${env.BUILD_NUMBER}"
    }

    stages {
        stage("Build") {
            steps {
                withMaven(maven: "maven"){
                    sh "mvn clean package"
                }
            }
        }
        stage("docker") {
            steps {
                sh 'docker-compose build'
                sh 'docker-compose push'
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