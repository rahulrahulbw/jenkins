pipeline {
    agent any

    stages {
        stage('checkout the code') {
            steps {
                git branch: 'main', url: 'https://github.com/rahulrahulbw/jenkins.git'
            }
        }
        stage('build the docker image') {
            steps {
                sh 'docker build . -t docker.io/opsharmabw/postgres:v1'
            }
        }
    }
}
