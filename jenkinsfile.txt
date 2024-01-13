pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/ramyachetty/javaproject.git'
            }
        }
        stage('Java') {
            steps {
                bat '''javac Hello.java
               java Hello'''
            }
        }
    }
}