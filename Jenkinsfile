pipeline {
    agent none
    stages {
        stage('Node Version') {
            agent {
                docker { image 'node:14-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
        stage('Git Version') {
            agent {
                docker { image 'alpine/git:v2.30.2' }
            }
            steps {
                sh 'git --version'
            }
        }
    }
}
