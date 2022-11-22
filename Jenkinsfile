pipeline{
    agent any
    stages{
        stage('clone'){
            steps{
                git 'https://github.com/devops090/Studentapp.git'
            }
        }
        stage('clean'){
            steps{
                sh 'mvn clean'
            }
        }
        stage('compile'){
            steps{
                sh 'mvn compile'
            }
        }
         stage('test'){
            steps{
                sh 'mvn test'
            }
        }
         stage('deploy'){
            steps{
                sh 'mvn deploy'
            }
        }
    }
}
