pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
         stage('build') {
            steps {
                echo 'deploy'
            }
        }
         stage('deploy') {
            steps {
                echo 'build'
            }
        }
         stage('test') {
            steps {
                echo 'test'
            }
        }
   }
