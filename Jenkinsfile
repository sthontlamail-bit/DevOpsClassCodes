pipeline
{
	agent any  
	stages
	tools {
		maven 'maven399'
	{
		stage('Code Checkout')
		{
			steps
			{
				git 'https://github.com/sthontlamail-bit/DevOpsClassCodes.git'
			}
		}
		
		stage('Code Compile')
		{
			steps
			{    

				sh 'mvn compile'
			}
		}

		stage('Code Test')
		{
			steps
			{
				sh 'mvn test'
			}
		}

		stage('Code package')
		{
			steps
			{
				sh 'mvn package'
			}
		}
     }
}

