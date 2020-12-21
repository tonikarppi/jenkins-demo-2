/* Requires the Docker Pipeline plugin */
node('docker') {
    checkout scm
    stage('Build') {
        docker.image('golang').inside {
            sh 'go version'
        }
    }
}