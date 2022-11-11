pipeline 
{
	agent any
    	environment
	{
		PACKAGE_VERSION="1.0.0.${BUILD_NUMBER}"
		JAR_DIR="${WORKSPACE}/testNG/target/testng-0.0.1-SNAPSHOT.jar"
  		APP_DEST_FILE="${WORKSPACE}/testNG/target/MyProjectPackage.${PACKAGE_VERSION}.tar"
	}
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
       			echo "jar creation completed"
			echo ${JAR_DIR} ${WORKSPACE}
			}
    		}
	}

}