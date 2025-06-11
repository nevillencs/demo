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
    }
}
