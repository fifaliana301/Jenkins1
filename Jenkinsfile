pipeline {
    agent any

    // options {
    //     paraellelAlwaysFailFast()
    // }

    stages {
        stage('build'){ 
            failFast true
            parallel{
                stage('build frotend'){
                    steps{
                        echo "build frontend"
                    }
                }
                stage('build backend'){
                    steps{
                        echo "build backend"
                    }
                }
            }
        }
        stage('deployement production'){
            steps{
                echo "deployement production"
            }
        }

    }
}