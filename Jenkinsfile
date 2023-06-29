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
                    
                } else {
                    echo "Build failed"
                    build 'Maven_proj'
                }
}
        }
    }
}
