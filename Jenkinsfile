pipeline {
    agent {
        docker { image 'node:14-alpine' }
    }
    stages {
        stage('Node Version') {
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
