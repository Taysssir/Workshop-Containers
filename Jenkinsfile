pipeline {
    agent {
        docker { image 'node:16' 
               args '-u root:root'
}
        }
    stages {
        stage('Node Version') {
            steps {
                sh 'node --version'
                sh 'git --version'
            }
        }
        stage ("cloning") {
            steps{
                echo "cloning"
               //sh "git clone https://github.com/contentful/the-example-app.nodejs.git"
            }
        }
        stage ("Install dependenciess"){
            steps{
                echo "installing dependencies"
                sh 'npm cache clean --force'
                //sh 'chown -R 126:130 "/.npm"'
                //sh "npm i npm@latest -g"
                sh "cd the-example-app.nodejs && npm install"
            }
        }
        stage ("Deploy"){
            steps{
                echo "start project"
                sh "cd the-example-app.nodejs && npm run start:dev &"
            }
        }
        stage ("Test"){
            steps{
                echo "verify"
                sh "curl  -L http://localhost:3000" 
                //sh "curl -L http://www.google.com" : works fine
            
            }
        }

      
    }
}
