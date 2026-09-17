pipeline {
    agent {
        label  'windows-agent'
    }
    stages {

        stage('Identify Branch') {
            steps {
                echo "================================"
                echo "Running Jenkins Multibranch Demo"
                echo "Branch: ${env.BRANCH_NAME}"
                echo "Job: ${env.JOB_NAME}"
                echo "Build Number: ${env.BUILD_NUMBER}"
                echo "================================"
            }
        }

        stage('Build') {
            steps {
                echo "Building branch: ${env.BRANCH_NAME}"
            }
        }

        stage('Test') {
            steps {
                echo "Testing branch: ${env.BRANCH_NAME}"
            }
        }
    }

    post {
        success {
            echo "Pipeline successful for ${env.BRANCH_NAME}"
        }

        failure {
            echo "Pipeline failed for ${env.BRANCH_NAME}"
        }
    }
}
