pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=rajbhushan -Dsonar.organization=rajbhushan -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0d692fbb26cf7e9d5528e58881398180d4bbc4a2'
			}
        } 
  }
}
