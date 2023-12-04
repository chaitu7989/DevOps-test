pipeline {
    agent any
    stages {
        stage('build and analyze') {
            steps {
                withSonarQubeEnv('sonar') {
                    sh 'mvn clean package sonar:sonar'
                }
            }
        }
        stage('sonar analysis') {
            steps {
                sh 'mvn sonar:sonar'
            }
        }
    }
}
