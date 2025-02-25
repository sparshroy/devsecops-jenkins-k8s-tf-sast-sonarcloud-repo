pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp101 -Dsonar.organization=asgbuggywebapp101 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1361a0bd51be3ae3806afb58bdc6a89522f6f303'
			}
        } 
  }
}
