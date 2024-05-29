pipeline {
    agent any
    
    tools {
        
        maven 'Maven'
    }

    stages {
        stage('Hello') {
            steps {
                sh 'mvn test' ; sh 'mvn install'
            }
        }
    }
}
