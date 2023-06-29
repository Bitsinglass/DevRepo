pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                              
            }
        }
        
    }
    post {
        always {
            script {
                 def buildStatus = currentBuild.result
                
                if (buildStatus == 'SUCCESS') {
                    echo "Build succeeded"
                    build 'Maven_proj'
                } else {
                    echo "Build failed"
                }
}
        }
    }
}
