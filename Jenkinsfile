pipeline {
    agent any
    stages {
        stage('git clone') {
            steps {
                git 'https://github.com/thomas-manoj/Studentapp.git'
            }
        }
        stage('validate') {
            steps {
                sh 'mvn validate'
            }
        }
         stage('clean') {
            steps {
                sh 'mvn clean'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}
