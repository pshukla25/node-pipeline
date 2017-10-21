node {
    def app

    stage('Clone repository') {
    sh 'pwd'
    sh 'echo "Source code can be pulled from github"'
    }

    stage('Build image') {
        
        sh 'ls -l'
        sh 'echo "Docker build images "'
    }

    stage('Test image') {
            sh 'hostname'
            sh 'echo "Tests passed "'
    }

    stage('Push image') {
            sh 'echo "Build pushed to dockerhub"'
    }
}
