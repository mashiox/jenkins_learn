pipeline {
    agent any //{ docker 'node:6.3' }
    stages {
        stage('Test') {
            steps {
                echo "I am in the test stage"
                echo 'This is a command in the Test step'
                timeout(time: 4, unit: 'SECONDS'){
                    echo 'Hey thar'
                }
            }
        }
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}
