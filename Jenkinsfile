pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=chrlwebapp_chrlwebapp -Dsonar.organization=chrlwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=640aef81f071dfc0b42a035bc52e26b99cd39d40'
			}
        } 
  }
}
