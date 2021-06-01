pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                withMaven(maven: 'maven-3.3.3') {
                    sh 'mvn clean'
                }
            }
        }
        stage('Install') {
            steps {
                withMaven(maven: 'maven-3.3.3') {
                    sh 'mvn install'
                }
           }
        }
        stage('Package') {
            steps {
                withMaven(maven: 'maven-3.3.3') {
                    sh 'mvn package'
                }
            }
        }
    }
}
