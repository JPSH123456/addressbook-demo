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
            
        }
    }

