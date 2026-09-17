pipeline {
    agent any

    stages {
        stage('Identify Branch') {
            steps {
                echo "Running branch: ${env.BRANCH_NAME}"
                echo "Job: ${env.JOB_NAME}"
                echo "Build: ${env.BUILD_NUMBER}"
            }
        }
    }
}