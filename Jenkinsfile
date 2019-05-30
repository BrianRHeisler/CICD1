pipeline {
    agent any

    stages {
        stage('Stage one') {
            steps {
                script {
                    docker.build "hello-world"

                    docker.withRegistry("https://957313429160.dkr.ecr.us-east-1.amazonaws.com/", "ecr:us-east-1:aws-role")  {
                        docker.image("hello-world").push("latest")
                    }
                }
            }
        }
    }
}
