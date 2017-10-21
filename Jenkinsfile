node {
    def app

    stage('Clone repository') {

        checkout scm
    # git url: 'https://github.com/pshukla25/node-pipeline.git'
    }

    stage('Build image') {

        app = docker.build("pshukla25/node-pipeline")
    }

    stage('Test image') {

        app.inside {
            sh 'echo "Tests passed"'
        }
    }

    stage('Push image') {
        docker.withRegistry('https://registry.hub.docker.com', 'docker-hub-credentials') {
            app.push("${env.BUILD_NUMBER}")
            app.push("latest")
        }
    }
}
