pipeline {
    agent any
  
    stages {
        stage('Test') {
            steps {
                sh "gradle clean test"
            }
  
            post {                
                // If Gradle was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                success {
                   echo 'success demo'
                }
            }
        }
    }
}
