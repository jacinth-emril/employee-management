pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Employee Management Application'
                sh 'mvn clean package'
            }
        }

        stage('Verify JAR') {
            steps {
                sh 'ls -lh target/*.jar'
            }
        }
    }
}
