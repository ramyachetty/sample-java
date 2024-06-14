pipeline {
    agent {
        label ('slave1')
    }

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/ramyachetty/javaproject.git'
            }
        }
        stage('Java'){
            steps {
                sh 'java Hello.java'
            }
        }
        
    }
}
