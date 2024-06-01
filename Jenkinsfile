pipeline {
    agent any
 tools {
        maven 'Maven'
    }
    
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

        stage (Test){

            when {
              expression {
                currentBuild.result == null || currentBuild.result == 'SUCCESS' 
              }
        }
             steps {
                 echo 'build sucess !!!'
                 
             }

            
        
    }
}
