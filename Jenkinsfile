pipeline {
      agent {
	     label "built-in"
	  }
	    stages {
	       stage ("compile stage"){
         		 steps {
                      sh "mvn clean compile"
		}				
      }		   
	        stage ("testing stage") {
			    steps {
		           sh "mvn test"
		   }		
        }
		    stage ("install stage"){
			    steps {
				   sh "mvn install"
			    }
			}	
	        stage ("deploy stage"){
	             steps {
			        sh "mvn deploy"
			}	 
		}		
	}	
}
