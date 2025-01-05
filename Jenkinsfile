pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6'
    }
    stages {
        stage('build') {
            steps {
                echo 'Compile app'
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                echo 'Run tests '
                sh 'mvn clean test'
            }
        }
        stage('package') {
            steps {
                echo 'Package'
                sh 'mvn pakcage -DskipTests'
            }
        }
    }
    post{
    always{
        echo 'pipeline completed'
        }
    }
}


