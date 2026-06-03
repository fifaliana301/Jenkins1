pipeline {
    agent {
        docker {
            image 'node:21-alpine'
        }
    }
    stages {
        stage('build'){ 
            steps {
                sh 'npm -v'
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
    }
}