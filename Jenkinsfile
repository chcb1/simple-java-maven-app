pipeline {
    agent any
    tools {
        maven 'Maven 3.14.0'
    }
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