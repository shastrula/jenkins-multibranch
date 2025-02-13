pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello, World!'
            }
        }
        stage("read file") {
            steps {
                script {
                    def file = readFile 'helloworld.yaml'
                    echo file
                }
            }
        }
    }
}