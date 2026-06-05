pipeline {
    agent any

    stages {
        stage('build'){ 
            steps {
                echo 'build !'
            }
        }

        stage('deployment production'){ 
            input {
                message "Voulez-vous déployer en production ?"
                ok 'déployer'
                submitter 'admin, devops'
                submitterParameter 'USER_SUBMIT'
                parameters {
                    string(name: 'VERSION', defaultValue: '1.0.0', description: 'Version à déployer')
                }
            }
            steps {
                echo "user: ${USER_SUBMIT}"
                echo "version: ${VERSION}"
                echo 'deployment production !'
            }
        }
    }
}