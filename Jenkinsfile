pipeline{
    agent{
        label 'slave1'
    } 
    stages{
        stage('git checkout'){
            steps{
                git 'https://github.com/JPSH123456/addressbook-demo.git'
            }
        }
        stage('build application'){
            steps{
                sh 'mvn install'
            }
        }
        stage('build docker images'){
            steps{
                sh 'docker build -t addressbook:2.0 .'
            }
        }
            
        }
    }

