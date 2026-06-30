node {
   stage('Checkout') {
        checkout scm
    }

   stage('Build Docker Image') {
        sh 'docker build -t resourcespace .'
    }

   stage('Run Container') {
    sh 'docker rm -f resourcespace || true'
    sh 'docker run -d --name resourcespace -p 8000:80 resourcespace'
}
}
