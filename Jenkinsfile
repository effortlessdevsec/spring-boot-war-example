pipeline {
    agent any
    
    tools {
        
        maven 'Maven'
    }

    stages {
        stage('Hello') {
            try{
steps {
                sh 'mvn test' ; sh 'mvn install'
            }

                catch {
                    echo 'error in building'
                }

                
            }
        }
    }
}
