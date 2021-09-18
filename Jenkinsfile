
pipeline {

    agent {
        docker { image 'node:14-alpine' }
    }
   tools {
      docker "Docker"
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
