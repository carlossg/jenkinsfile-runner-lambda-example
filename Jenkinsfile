pipeline {
    agent any
    environment {
        PATH = "/usr/local/bin:$PATH"
        JAVA_HOME = '/opt/usr/lib/jvm/java-openjdk'
    }
    stages {
        stage('Build') {
            steps {
                sh 'git clone https://github.com/carlossg/jenkinsfile-runner-lambda-example.git'
                echo 'Hello world!'
                sh 'mvn -Duser.home=/tmp clean package'
            }
        }
    }
}
