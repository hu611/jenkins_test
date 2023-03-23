pipeline {
    agent none
    stages{
        stage('start') {
          agent{
            label "master"
          }
            steps {
                echo "start passed successfully"
            }
        }
        stage('compile') {
          agent{
            label "master"
          }
            steps {
                echo "compile passed successfully"   
            }
            
        }
        stage('deploy') {
          agent{
            label "master"
          }
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
