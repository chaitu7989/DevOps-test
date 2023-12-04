pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package -DskipTests=true'
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
