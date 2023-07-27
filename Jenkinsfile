pipeline{
    agent{
        label 'slave1'
    } 
    stages{
        stage('git checkout'){
            steps{
                git 'https://github.com/JPSH123456/game-of-life.git'
            }
        }
        stage('build application'){
            steps{
                sh 'mvn install'
            }
        }
      
            
        }
    }

