pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=chrlwebapp -Dsonar.organization=chrlwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2edd4cab885b04ed80349b4df5ba9f1bb2515536'
			}
        } 
  }
}
