pipeline {
    agent any
    stages {
        stage('build and analyze') {
            steps {
                    sh 'mvn clean package'
                }
            }
         stage('build and analyze') {
            steps {
                    sh 'mvn clean verify sonar:sonar \
                       -Dsonar.projectKey=test \
                        -Dsonar.projectName='test' \
                        -Dsonar.host.url=http://10.1.151.15:9000 \
                        -Dsonar.token=sqp_a5b9838ffd8eef4459ca608607756c1a73c84f77'
                }
            }
        }
}

