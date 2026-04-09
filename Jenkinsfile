pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/NishitaVedpathak03/maven-jenkins-demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}