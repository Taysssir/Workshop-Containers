pipeline {
    agent {
        docker { image 'node:16' }
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
