pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                // Checkout specific branch from Git
                git branch: 'master', 
                    url: 'https://github.com/Hassan-khan-007/hello-world-java.git'
            }
        }

        stage('Build') {
            steps {
                // Compile HelloWorld.java
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                // Run the compiled class
                sh 'java HelloWorld'
            }
        }
    }
}
