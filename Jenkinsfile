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
                sh 'docker build -t jpsh123456/addressbook:2.0 .'
                sh 'docker run -itd -p 8090:8080 jpsh123456/addressbook:2.0'
            }
        }
            
        }
    }

