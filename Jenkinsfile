pipeline {
    agent any

tools {
    maven '3.9.9'
}

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
                    sh 'java -jar target/hello-world-1.0-SNAPSHOT.jar'
                }
            }
        }
    }
}
