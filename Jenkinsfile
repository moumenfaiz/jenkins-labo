pipeline {
    agent any 
    stages {
        stage('clone') {
            steps{
                sh "rm -rf *"
                sh "git clone https://github.com/moumenfaiz/jenkins-labo.git"
            }
        }
        stage('build') {
            steps{
                sh "cd jenkins-labo/ && javac Main.java"
            }
        }
        stage('run') {
            steps{
                sh "cd jenkins-labo/ && java Main"
            }
        }
    }
}

