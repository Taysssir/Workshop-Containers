pipeline {
    agent {
        docker { image 'node:14-alpine' }
        }
    stages {
        stage('Node Version') {
            steps {
                sh 'node --version'
                sh 'git --version'
            }
        }

      
    }
}
