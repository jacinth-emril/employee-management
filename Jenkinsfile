pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Employee Management Application'
                sh './build.sh'
            }
        }

        stage('Verify JAR') {
            steps {
                sh 'ls -lh target/*.jar'
            }
        }
    }
}
