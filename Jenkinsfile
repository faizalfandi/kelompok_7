pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/faizalfandi/kelompok_7.git'
            }
        }
        stage('Deploy') {
            steps {
                sh 'ansible-playbook -i inventory.ini ansible/deploy_nginx.yml'
            }
        }
    }
}
