
pipeline {

    agent {
        docker { image 'node:14-alpine' }
    }
   tools {
      docker "docker"
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
