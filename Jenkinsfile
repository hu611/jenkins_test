pipeline {
    agent any
    stages{
        stage('start') {
         
            steps {
                echo "start passed successfully"
            }
        }
        stage('compile') {
          
            steps {
                echo "compile passed successfully"   
            }
            
        }
        stage('deploy') {
          
            steps {
                echo "deploy"    
            }   
            
        }
    }
    
    post {
        always {
            echo "This will always run"
        }
        success {
            echo "This will run only if successful"
        }
        failure {
            echo "This will run only if failed"
        }
    }
}
