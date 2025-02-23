pipeline {
<<<<<<< HEAD
    agent any

    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }

    stages {

        stage('GIT') {
            steps {
                git branch: 'main', url: 'https://github.com/eyachamekh/devops.git'
            }
        }

        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }

    }
}
=======

 agent any

 environment {
         JAVA_HOME = "/usr/lib/jvm/java-17-openjdk-amd64/"
         M2_HOME = "/opt/apache-maven-3.6.3"
         PATH = "$M2_HOME/bin:$PATH"
     }

 stages {

 stage('GIT') {

           steps {

               git branch: 'main',

             https://github.com/eyachamekh/devops.git

          }

     }

 stage ('Compile Stage') {

 steps {

 sh 'mvn clean compile'

 }

 }
 stage('SonarQube analysis') {
steps{
sh 'mvn sonar:sonar'
}
 }
>>>>>>> origin/main
