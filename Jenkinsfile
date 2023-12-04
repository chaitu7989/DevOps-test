pipeline {
    agent any
    stages {
        stage('build and analyze') {
            steps {
                    sh 'mvn clean package'
                }
            }
        }
        stage('sonar analysis') {
            steps {
                withSonarQubeEnv('sonar') {
                sh 'mvn sonar:sonar'
            }
        }
    }
}
