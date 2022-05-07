pipeline
 {
  agent any
  stages{
	 stage('Build Application'){
	  steps{
	  bat 'mvn clean install'
	  }	 
	  }
	  
	 stage('Munit Test Application'){
	  steps{
	  bat 'mvn clean test'
	  }	 
	  }
	  
	 stage('Deploy Application to Mulesoft Cloudhub'){
	  steps{
	  bat 'mvn clean package deploy -DmuleDeploy'
	  }
	 }
	 
	}
 }
