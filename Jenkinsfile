pipeline
{
  agent any
  	stages{
  	stage('Build Application'){
  	steps{
  	bat 'mvn clean install'
  	   	}
  	}
  	
  	  	stage('Deploy Application to Mulesoft Cloud Hub'){
  	  	steps{
  			bat 'mvn package deploy -DmuleDeploy'
  			}
  	}
  	
  	
  	  	  	stage('Perform Regression Testing'){
  	  	  	steps{
  			bat 'C:\\Users\\asus\\AppData\\Roaming\\npm\\newman run C:\\Users\\asus\\Documents\\Mulesoft\\TimeZOne.postman_collection.json --disable-unicode'
  			}
  	}
  	
  	
  	}
  	

}

