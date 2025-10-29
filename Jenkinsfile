pipeline{
    stages{
        stage("build"){
            sh ."docker build -t fullcicd:latest ."
            sh . "docker tag fullcicd:latest akkolluru/fullcicd:latest"
            sh . "docker login -u akkolluru"
            sh . "docker push akkolluru/fullcicd:latest"
        }
    }
}