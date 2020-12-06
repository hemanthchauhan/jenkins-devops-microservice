pipeline {
	agent any
	//agent { docker{ image 'node:15.3'}}
	stages{
		stage('Build'){
			steps{
				//sh 'mvn --version'
				//sh 'node --version'
				echo "Build"
				echo "Path - $PATH"
				echo "Build Number - $env.BUILD_NUMBER"
				echo "Build ID - $env.BUILD_ID"
				echo "Job Name - $env.JOB_NAME"
				echo "Node Name - $env.NODE_NAME"
				echo "Build WOrkspace - $env.WORKSPACE"
				echo "Build Url - $env.BUILD_URL"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	} 
	post {
		always{
			echo 'I run always!'	
		}
		success{
			echo 'I run if the build is successful'
		}
		failure{
			echo 'I run on failures'
		}
	}	
}
