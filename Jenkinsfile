pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "verify Ansible is installed"'
                sh '''
                    echo "Checking Ansible"
                    ls -lah
                '''
                sh 'ansible --version'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Ansible ping localhost"'
                sh 'ansible localhost -m ping > /tmp/myoutput.txt'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Ansible ping localhost"'
                sh 'ls -l /tmp/myoutput.txt'
                sh 'cat /tmp/myoutput.txt'
            }
        }
    }
}
