pipeline {
    agent {
        label 'slaveNode1'
    }
    stages {
        stage('init') {
            steps {
                echo 'initializing'
                script {
                    // Replace this with your actual 'terraform init' command
                    sh 'terraform init'
                }
            }
        }
        stage('validate') {
            steps {
                echo 'validating'
            }
        }
        stage('plan') {
            steps {
                echo 'planning'
                script {
                    // Replace this with your actual 'terraform plan' command
                    sh 'terraform plan'
                }
            }
        }
        stage('apply') {
            steps {
                echo 'applying'
                script {
                    // Replace this with your actual 'terraform apply' command
                    sh 'terraform apply -auto-approve'
                }
            }
        }
    }
}
