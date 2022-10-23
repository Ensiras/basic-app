pipeline {
    agent any

    stage("checkout scm") {
        steps {
            echo "hello there"
            checkout([$class: 'GitSCM', branches: [[name: '*/develop']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-key', url: 'git@github.com:Ensiras/basic-app.git']]])
        }
    }
}