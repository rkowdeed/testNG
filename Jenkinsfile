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
			//bat 'cd C:/Users/P7167137/.jenkins/workspace/testNG/target/'
			bat 'copy target\/testng-0.0.1-SNAPSHOT.jar /Y D:'
			}
    		}
	}

}