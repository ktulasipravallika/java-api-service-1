pipeline {
	agent any 
		stages {
			stage('getCode') {
			    steps{
				  git branch: 'main', url: 'https://github.com/ktulasipravallika/java-api-service-1.git'
				  sh 'mvn compile'
				  echo "Compilation completed successfully"
				}
			}
			stage('test') {
                 steps {
	                sh 'mvn test'
	                echo "Testing completed successfully"
		            sh 'mvn clean package'
                    echo "Artifact Created Successfully"
		         }
			}
	    }
	}

