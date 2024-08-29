pipeline {
    agent any
    
    stages {
        stage('Compile and Clean') { 
            steps {

                bat "mvn clean compile"
            }
        }
       
		
        
        stage('SonarQube'){
			steps{
				  bat "mvn clean install"
			
			}
   		}
        
     

        stage('Build Docker image'){
            steps {
                bat "mvn test"
         
           }
        }

        stage('Docker Login'){
            
            steps {
              
                }
            }                
        

        stage('Docker Push'){
            steps {
       
            }
        }
        
        stage('Docker deploy'){
          steps {
               
           
            }
        }

        
      
     
    }
}
