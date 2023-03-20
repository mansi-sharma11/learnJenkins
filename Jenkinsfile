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
                    failed()
                }
            }
            steps {
                sh 'mvn test'
            }
        }
    }
}
