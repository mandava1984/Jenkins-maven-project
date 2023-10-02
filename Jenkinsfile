pipeline {
    agent any 
    stages {
        stage(‘clean ‘and compile) { 
            steps {
                sh "mvn clean c”compile 
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
    }
}
