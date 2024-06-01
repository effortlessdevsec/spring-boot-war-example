pipeline {
    agent any

    

    stages {
        stage('Hello') {
            steps {
                script {
                    try {
                        sh 'mvn test'
                        sh 'mvn install'
                    } catch (Exception e) {
                        echo 'Error in building'
                        error 'Build failed'
                    }
                }
            }
        }
    }
}
