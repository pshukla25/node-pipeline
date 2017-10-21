node {
    def app

    stage('Clone repository') {
    sh 'echo "Tests passed 1"'
    }

    stage('Build image') {

        sh 'echo "Tests passed 2"'
    }

    stage('Test image') {

        app.inside {
            sh 'echo "Tests passed 3"'
        }
    }

    stage('Push image') {
            sh 'echo "Tests passed 4"'
    }
}
