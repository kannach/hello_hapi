#!/usr/bin/env groovy

pipeline {

    agent any

    stages {
         stage('install') {
            steps {
                echo 'Installing node...'
                sh 'sudo docker pull node'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'sudo npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'sudo npm test'
            }
        }
    }
}
