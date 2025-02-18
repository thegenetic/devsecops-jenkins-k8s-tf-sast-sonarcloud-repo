pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=thegeneticbugywebapp -Dsonar.organization=thegeneticbugywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fe2233f7974aa6cd1e3055eedc30aa4523c95947'
			}
        } 
  }
}
