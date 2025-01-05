pipeline {
    agent any

    stages {
        stage('one') {
            steps {
                echo 'step one'
                sh 'mvn compile'
            }
        }
        stage('two') {
            steps {
                echo 'step 2'
                sh 'mvn compile'
            }
        }
        stage('three') {
            steps {
                echo 'step 3'
                sh 'mvn compile'
            }
        }
    }
}
