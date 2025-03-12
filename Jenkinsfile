pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gBlengio -Dsonar.organization=gBlengio -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e1d0b9d824f9575e0234cfeed3408bf9683ee436'
			}
        } 
  }
}
