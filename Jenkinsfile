pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
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
