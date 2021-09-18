
pipeline {
   tools {
      docker "Docker"
    }
    agent {
        docker { image 'node:14-alpine' }
    }

    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
