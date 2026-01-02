pipeline{
    agent any

    tools{
        maven 'MAVEN_HOME'
    }
    stages{
        stage('Hello My Java App'){
            steps{
                echo 'Hello My Java App'
            }
        }
        stage('Cloning the repo'){
            steps{
                git branch:'main', url: 'https://github.com/shohail-Dev/spring-boot-hello-world.git'
            }
        }
        stage ('Test'){
            steps{
                bat 'mvn test'
            }
        }
        stage('Code Restoration'){
            steps{
                bat 'mvn clean'
            }
        }
        stage('Artifact'){
            steps{
                bat 'mvn clean install'
            }
        }
    }
}