pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testasgbuggywebapp -Dsonar.organization=testasgbuggywebapp -
Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c6b186c7f4615522908ebc6d747653a25dd294ce'
			}
        } 
  }
}
