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
        sh 'mvn install'
      }
    }
    stage('deploy application'){
      steps{
        sh 'cp -r /root/.jenkins/workspace/newjob/target/addressbook-2.0.war /opt/tomcat/apache-tomcat-9.0.78/webapps/''
      }
    }
  }
 }
