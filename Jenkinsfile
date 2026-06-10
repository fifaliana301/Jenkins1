pipeline {
    agent any

    tools {
        gradle 'gradle9.6'
        nodejs 'node26'
    }

    stages {
        stage('build'){
            steps {
               sh 'gradle -v'
               sh 'node -v'
            }
        }
    }
}