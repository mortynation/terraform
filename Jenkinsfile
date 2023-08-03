pipeline {
    agent {label 'slaveNode1'}
    stages('init') {
        echo 'initializing'
        script {
            dir() {
                sh 'terraform init'
            }
        }

    }
    stages('validate') {
        echo 'validating'
    }
    stages('plan') {
        echo 'planning'
        script {
            dir() {
                sh 'terraform plan'
            }
        }

    }
    stages('apply') {
        echo 'applying'
        script {
            dir() {
                sh 'terrafrom apply -auto-approve'
            }
        }
    }
}