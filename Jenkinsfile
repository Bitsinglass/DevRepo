pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                        echo "hariom"      
               
            }
        }
        
    }
    post {
        always {
            script {
                 def buildStatus = currentBuild.result
                
                if (buildStatus == 'SUCCESS') {
                    echo "Build succeeded"
                    build 'Test_Automation_Build'
                } else {
                    echo "Build failed"
                    
                }
}
        }
    }
}
