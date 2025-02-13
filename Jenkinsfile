pipeline {
    agent any

    stages {
        stage('Maven Build') {
            steps {
                dir('hello-world') {
                    sh 'mvn clean package'
                }
            }
        }

        stage('Run Jar') {
            steps {
                dir('hello-world') {
                    sh 'java -jar target/hello-world-0.0.1-SNAPSHOT.jar'
                }
            }
        }
    }
}
