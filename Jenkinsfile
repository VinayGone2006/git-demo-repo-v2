pipeline {
    agent any

    tools {
        maven 'Maven-3'
    }

    stages {
        stage('Compile') {
            steps {
                echo 'Compiling the code...'
                sh 'mvn compile'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the package...'
                sh 'mvn package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'
            }
        }
    }
}
