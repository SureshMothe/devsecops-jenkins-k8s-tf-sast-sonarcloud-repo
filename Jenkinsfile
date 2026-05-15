pipeline {
  agent any
  tools { 
        maven 'Apache_Maven_3.8.4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sureshmothe -Dsonar.organization=SureshMothe -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=0b49f1f2e759ffb1ecf87c19d294bd1e6fa7e6bb'
			}
        } 
  }
}
