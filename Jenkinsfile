pipeline
{
 agent any
 stages{
  stage('Build_Cicd'){
  steps{
  bat 'mvn clean install'
  }
  }
  
   stage('Deploy_Cicd_Application'){
   steps{
  bat 'mvn deploy -DmuleDeploy'
  }
  }
    stage('Testing_Cicd'){
    steps{
  bat 'newman run D:\\newman\\Employee-API.postman_collection.json --disable-unicode'
  }
  }
  
 }
 
}