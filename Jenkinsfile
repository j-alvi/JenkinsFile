pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "verify Ansible is installed!!!"'
                sh '''
                    echo "Checking $TEST"
                    ls -lah
                '''
                sh 'ansible --version'
            }
        }
    }
}
