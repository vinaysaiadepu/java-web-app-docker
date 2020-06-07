pipeline{
	agent any
	tools {
    maven 'Maven'
  }
	stages{
		stage('SCM Checkout'){
			steps{
				git branch: 'devops/test',
                		url: 'https://github.com/vinaysaiadepu/java-web-app-docker.git'
			}
		}
		

		stage('Stage1'){
                        steps{
                                echo 'this is stage1'
                        }
                }

		stage('Stage2'){
			when {
			
					branch 'master2'
			
		}
                        steps{
                                echo 'this is not master branch'
                        }
                
		}

		
        stage('Build') {
            steps {
                //def mavenHome= tool name: "Maven", type: "maven"
        
        sh 'mvn install'
            }
        }
}
}
