pipeline{
 tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
     agent any
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	  git 'https://github.com/1993Abhijit/job2.git'
	   }
	                  }
	
	   stage("compile"){
	    steps{
		 sh 'mvn compile'
		}
		}
          stage("test"){
	    steps{
		 sh 'mvn test'
		}
		}

        stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
		
		stage("deploy"){
	    steps{
		 echo "deploy my app"
		}
		}
		  stage("install"){
	    steps{
		 echo "install my app"
		}
		}
		  


	  }
	}

