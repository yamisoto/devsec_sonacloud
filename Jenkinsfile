pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cgtlxsonacloud -Dsonar.organization=cgtlxsonacloud -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=50ad8a658cefa31683fd5e88066e504fef4abd69'
			}
        } 
  }
}
