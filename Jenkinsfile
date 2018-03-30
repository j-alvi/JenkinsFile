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
        }
    }
}
