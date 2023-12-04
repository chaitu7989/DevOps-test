pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                withSonarQubeEnv('sonar') {
                sh 'mvn clean package sonar:sonar'
            }
        }
    }
     stages {
        stage('build') {
            steps {
                sh 'mvn sonar:sonar
            }
        }
    }
}
