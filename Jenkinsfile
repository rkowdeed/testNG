pipeline 
{
	agent any
	stages
	{
    		stage('Preparation') 
		{
        		steps
			{
			git 'https://github.com/rkowdeed/testNG.git'
			}
    		}
    		stage('install')
		{
			steps
			{
        		bat 'mvn clean install' // Dependency Installation stage
    			}
		}    
    		stage('Deploy') 
		{
			steps
			{
			bat 'cd C:/Users/P7167137/.jenkins/workspace/testNG/target/ move testng-0.0.1-SNAPSHOT.jar D:/'
			//bat 'move testng-0.0.1-SNAPSHOT.jar D:/'
			}
    		}
	}

}