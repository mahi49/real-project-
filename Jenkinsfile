pipeline {
    agent any
    stages {
      stage('checkout') {
            steps {
              sh'checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'mahi49', url: 'https://github.com/mahi49/real-project-.git']]])'
            }
        }
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
