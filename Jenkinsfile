pipeline {
    agent any
    stages {
        stage('init') {
            steps {
                echo '${env.BRANCH_NAME}'
            }
        }
        stage('Build Master') {
            when {
                branch 'master'
            }
            steps {
                echo 'Building master'
            }
        }
        stage('Build Dev') {
           when {
                    branch 'develop'
                }
            steps {
                echo 'Building dev'
            }
        }
    }
}
