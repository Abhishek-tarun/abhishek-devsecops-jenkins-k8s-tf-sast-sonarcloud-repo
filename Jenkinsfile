pipeline {
    agent any
    tools {
        maven 'Maven_3_2_5'
    }
    stages {
        stage('COmpileandRunSonarAnalysis') {
            steps {
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=abhishek-tarun_asbuggywebapp -Dsonar.organization=abhishek-tarun -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0389828f7ffe32a1b25ec2642230f04e5155a8f0'
            }
        }
    }
}
