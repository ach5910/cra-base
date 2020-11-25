pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            steps {
                sh "curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -"
                sh "echo 'deb https://dl.yarnpkg.com/debian/ stable main' | tee /etc/apt/sources.list.d/yarn.list"
                sh "apt update && apt install yarn"
                sh "yarn"
            }
        }
    }
}