pipeline {
    agent any
    stages {
            stage('Downloading the Dependencies'){
                steps {
                    sh "npm install"
                }
            }

        stage('Lint Checks') {
            steps {
                sh "echo installing jslint"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js"
            }
        }
    }  // End of stages
}