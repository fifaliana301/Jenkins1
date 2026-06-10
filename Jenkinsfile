pipeline {
    agent any

    stages {
        stage('Build'){
            steps {
                echo 'echo hello > world.txt'
                archiveArtifacts(artifacts: '*.txt')
            }
        }
    }
}