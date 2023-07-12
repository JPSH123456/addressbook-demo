 pipeline{
  agent{
    label 'slave-1'
  }
  stages{
    stage('git checkout'){
      steps{
        git 'https://github.com/JPSH123456/addressbook-demo.git' 
      }
    }
    stage('build application'){
      steps{
        sh 'mvn clean install'
      }
    }
  }
 }
