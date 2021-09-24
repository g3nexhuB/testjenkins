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
                sh 'ansible all -b -a "ls -ld /root" -i "ubuntu," '
                }
            }
        }
}
