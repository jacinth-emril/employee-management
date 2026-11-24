pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Employee Management Application'
                sh 'mvn clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Application Tests'
                sh 'mvn test'
            }
        }

        stage('Verify JAR') {
            steps {
                sh 'ls -lh target/*.jar'
            }
        }
    }
}
