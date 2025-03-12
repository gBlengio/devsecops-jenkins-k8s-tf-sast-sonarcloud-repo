pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-jenkins-k8s-tf-sast-sonarcloud-repo -Dsonar.organization=gblengio -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=86546a3cd83a6e7b60c6f0931c8ebcea77337cfb'
			}
        } 
  }
}
