pipeline {
    agent any

    stages {
        stage('Stage one') {
            steps {
                script {
                    docker.build "demo1"
                }
            }
        }
    }
}
