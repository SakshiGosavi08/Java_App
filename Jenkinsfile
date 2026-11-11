pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                // Pulls code from the repository configured in the Jenkins job
                checkout scm
            }
        }

        stage('Compile Java Program') {
            steps {
                // Compiles HelloWorld.java into HelloWorld.class
                sh 'javac HelloWorld.java'
            }
        }

        stage('Execute Application') {
            steps {
                // Runs the compiled Java class
                sh 'java HelloWorld'
            }
        }
    }
}
