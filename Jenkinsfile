pipeline {
    agent any
    environment {
        PATH = "/opt/apache-maven-3.8.1/bin/:$PATH"
    }

    stages {
        stage('fetch') {
            steps {
                git 'https://github.com/nihaldevops/simple-app.git'
            }
        }
        stage('package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}





  
