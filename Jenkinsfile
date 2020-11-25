pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'sudo chown -R 501:20 "/.npm"'
                sh 'npm install -g yarn'
                sh 'yarn -v'
            }
        }
    }
}