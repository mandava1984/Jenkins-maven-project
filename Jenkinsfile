pipeline {
    agent any 
    stages {
        stage('clean and compile') { 
            steps {
                sh "mvn clean compile"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test" 
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
        stage('Archive') { 
            steps {
                archiveArtifacts '**/target/*.jar'
            }
        }
    }
}
