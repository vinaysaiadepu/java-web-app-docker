pipeline{
	agent any
	stages{
		stage('SCM Checkout'){
			steps{
				git branch: 'master',
                		url: 'git@github.com:vinaysaiadepu/java-web-app-docker.git'
			}
		}
		

		stage('Stage1'){
                        steps{
                                echo 'this is stage1'
                        }
                }

		

	}
}
	
