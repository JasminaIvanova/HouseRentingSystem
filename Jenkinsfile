pipeline {
    agent any

    stages {
        stage('Restore') {
            steps {
                sh 'dotnet restore'
            }
        }

        stage('Start Application') {
            steps {
                sh 'dotnet build'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'dotnet test'
            }
        }
    }
}
