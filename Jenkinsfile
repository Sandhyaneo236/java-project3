pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Sandhyaneo236/java-project3.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing done'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp target/classes Main'
            }
        }
    }
}
