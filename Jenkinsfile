pipeline {
    agent any

    tools {
        gradle 'gradle9.6'
    }

    stages {
        stage('build'){
            steps {
               sh 'gradle -v'
            }
        }
    }
}