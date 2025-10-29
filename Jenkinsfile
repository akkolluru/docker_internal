pipeline {
    stages {
        stage('build'){
            steps {
            sh "docker build -t fullcicd ."
            sh "docker run -f -p fullcicd"
            sh "docker tag fullcicd akkolluru/fullcicd:latest"
            sh "docker login -u akkolluru "
            sh "docker push akkolluru/fullcicd:latest"
            }
        }
    }
}