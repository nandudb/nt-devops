<<<<<<< HEAD
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'uname -a'
                sh 'echo This is Testing branch!'
=======
podTemplate(containers: [
    containerTemplate(
        name: 'maven', 
        image: 'maven:3.8.1-jdk-8', 
        command: 'sleep', 
        args: '30d'
        ),
  ]) {

    node(POD_LABEL) {
        stage('Get a Maven project') {
            git 'https://github.com/dlambrig/simple-java-maven-app.git'
            container('maven') {
                stage('Build a Maven project') {
                    sh '''
                    echo "maven build"
                    mvn -B -DskipTests clean package
                    '''
                    }
>>>>>>> 6c729f903a99a458385f41103c25a62f77f0796a
            }
        }
