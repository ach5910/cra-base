pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'npm install -g yarn'
                sh 'yarn -v'
            }
        }
    }
}