pipeline {
    agent any
    stages {
        stage('compile') {
            steps {
                echo 'mvn compile'
            }
        }
        stage ('validate') {
            steps {
                echo 'mvn validate'
            }

        }
        stage ('test') {
            steps {
                echo 'mvn test'
            }
        }
         stage ('package') {
            steps {
                echo 'mvn package'
        
            }

         }    


    }
}    
