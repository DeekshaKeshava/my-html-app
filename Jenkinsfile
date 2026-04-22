pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/DeekshaKeshava/my-html-app.git'
            }
        }

        stage('Run Server') {
            steps {
                bat 'start cmd /c python -m http.server 8081'
            }
        }
    }
}