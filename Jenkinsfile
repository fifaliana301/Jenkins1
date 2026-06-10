pipeline {
    agent any

    stages {
        stage('build and test') {
            matrix{
                axes {
                    axis {
                        name 'PLATEFORM'
                        values 'linux', 'macos', 'windows'
                    }
                    axis {
                        name 'BROWSER'
                        values  'firefox', 'chrome', 'safari'
                    }
                }
                stages {
                    stage('build') {
                        steps {
                            echo "Building on ${PLATEFORM} with ${BROWSER}"
                            // Add build steps here
                        }
                    }
                    stage('test') {
                        steps {
                            echo "Testing on ${PLATEFORM} with ${BROWSER}"
                            // Add test steps here
                        }
                    }
                }
            }
        }
    }
}