pipeline{
 tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
     agent any
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git credentialsId: 'jenkins', url: 'https://github.com/1993Abhijit/jenkins2.git'
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


	  }
	}

