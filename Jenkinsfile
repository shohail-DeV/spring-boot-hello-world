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
                git 'https://github.com/shohail-Dev/spring-boot-hello-world.git
'
            }
        }
    }
}