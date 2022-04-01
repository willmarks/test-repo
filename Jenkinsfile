pipeline {
    agent any
    stages {
        stage('Version File') {
            steps {
                sh 'echo "Writing Version File"'
                sh '''
                    echo '{"repo1":"f0c8abb8e7df32f2b3a91e0268b90b96c5f23be9","repo2":"f0c8abb8e7df32f2b3a91e0268b90b96c5f23be9"}' > version.json
                '''
                archiveArtifacts artifacts: './version.json', allowEmptyArchive: 'true'
            }
        }
    }
}
