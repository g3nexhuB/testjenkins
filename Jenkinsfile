pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "testing"
                sh 'whoami'
                sh 'ls -lahtr'
                sh 'pwd'
                }
            }
        stage('build') {
            steps {
                echo "ansible test"
                sh 'ansible-playbook genex-playbook.yml -i 'ubuntu,' 
                }
            }
        }
}
