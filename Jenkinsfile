pipeline {
    agent any
    tools {
        gradle 8.3 
    }
    stages {        
        stage('Build Image') {
            steps {
                sh 'gradle init'
                sh "echo 'building..'"
               
                withGradle {
                   sh 'gradle wrapper build'
                }
                
            }
        }
}
}
