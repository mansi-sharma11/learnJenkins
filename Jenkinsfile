pipeline {
    agent any
    
    stages {
        stage('Compile') {
            steps {
                withMaven( maven: 'maven3'){
                sh 'mvn compile'
            }
        }
    }
}
                          }
