pipeline{
  agent any {
    stages{
      stage('sonar quality check'){
        agent{
          docker{
            iamge 'maven
          }
        }
        steps{
          script{
            withSonarQubeEnv(credentialsId: 'sonar-token') 
            sh 'maven clean package sonar:sonar'
          }
        }
      }
    }
  }
}
  
