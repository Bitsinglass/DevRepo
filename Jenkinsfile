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
                
                if (buildStatus == 'SUCCESSs') {
                    echo "Build succeeded"
                    
                } else {
                    echo "Build failed"
                    
                }
}
        }
    }
}
