pipeline {
    agent any
    stages {
        stage('Version File') {
            steps {
                sh 'echo "Writing Version File"'
                sh '''
                    echo '{"repo1":"sha1","repo2":"sha2"}' > version.json
                '''
                archiveArtifacts artifacts: './version.json', allowEmptyArchive: 'true'
            }
        }
    }
}
