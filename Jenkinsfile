pipeline {
    agent any
    //options { skipDefaultCheckout() }

    stages {
        stage('Source') {
            steps {
                echo "Stage: ${env.STAGE_NAME}"
                echo "Build Number: ${env.BUILD_DISPLAY_NAME}"
                echo "Jenkins Build URL: ${env.BUILD_URL}"
            }
        }
        stage('Test') {
            steps {
                echo "Stage: ${env.STAGE_NAME}"
                echo "Find the Jenkinsfile from Git ${env.GIT_URL} (Branch ${env.GIT_BRANCH})"
            }
        }
        stage('Deploy') {
            steps {
                echo "Stage: ${env.STAGE_NAME}"
                echo "Running on Jenkins version ${env.JENKINS_VERSION} in ${env.WORKSPACE}"
            }
        }
    }
}