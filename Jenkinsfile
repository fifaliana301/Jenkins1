pipeline {
    agent any

    tools {
        gradle 'gradle9.6'
        nodejs 'node22' 
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