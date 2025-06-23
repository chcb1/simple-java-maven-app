pipeline {
    agent any
    stages {
        stage('Install dependencies') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }

        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}