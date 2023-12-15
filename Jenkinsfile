pipeline {
    agent {
        label 'slave2'
    }

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/ramyachetty/javaproject.git'
            }
        }
        stage('execute') {
            steps {
                sh '''javac Hello.java
                       java Hello'''
            }
        }
    }
}
