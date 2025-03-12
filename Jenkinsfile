pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-jenkins-k8s-tf-sast-sonarcloud-repo -Dsonar.organization=gblengio -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=15267064b724131f11a92ee7a6384fc15da51e69'
			}
        } 
  }
}
