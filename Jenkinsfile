pipeline {
    agent { docker { image 'maven:3.9.9-eclipse-temurin-21-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'echo $JAVA_HOME'
                sh 'cd ~'
                sh 'touch temp && echo "This is me" > temp'
                sh 'cat temp'
            }
        }
    }
}
