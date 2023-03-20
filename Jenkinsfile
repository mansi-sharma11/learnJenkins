pipeline {
    agent any
    
    stages {
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            when {
                not {
                  echo 'IN NOT BLOCK'
                }
            }
            steps {
                sh 'mvn test'
            }
        }
    }
}
