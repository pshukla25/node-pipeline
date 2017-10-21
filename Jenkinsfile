node {
    def app

    stage('Clone repository') {
    sh 'echo "Tests passed 1"'
    #    checkout scm
    #git url: 'https://github.com/pshukla25/node-pipeline.git'
    }

    stage('Build image') {

        #app = docker.build("pshukla25/node-pipeline")
        sh 'echo "Tests passed 2"'
    }

    stage('Test image') {

        app.inside {
            sh 'echo "Tests passed 3"'
        }
    }

    stage('Push image') {
        #docker.withRegistry('https://registry.hub.docker.com', 'docker-hub-credentials') {
        #    app.push("${env.BUILD_NUMBER}")
        #    app.push("latest")
        #}
            sh 'echo "Tests passed 4"'
    }
}
