pipeline {
    agent {
        any {
            image 'maven:3.8.5-openjdk-17'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage("Build") {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}