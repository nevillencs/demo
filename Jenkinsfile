pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Build with Maven') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Cleanup') {
            steps {
                echo 'Cleaning up workspace...'
                deleteDir() // Deletes all files in the current workspace
            }
        }
    }
}
