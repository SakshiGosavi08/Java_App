pipeline {
    agent any

    tools {
        // Matches the name you provided in Manage Jenkins -> Tools
        jdk 'JDK-17'
    }

    stages {
        stage('Pull Code') {
            steps {
                checkout scm
            }
        }

        stage('Compile Java Program') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }

        stage('Execute Application') {
            steps {
                sh 'java HelloWorld'
            }
        }
    }
}
