node {
   stage('Checkout') {
        checkout scm
    }

   stage('Build Docker Image') {
        sh 'docker build -t resourcespace .'
    }
}
