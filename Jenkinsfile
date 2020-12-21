/* Requires the Docker Pipeline plugin */
node {
    checkout scm
    stage('Build') {
        docker.image('golang').inside {
            sh 'go version'
        }
    }
}