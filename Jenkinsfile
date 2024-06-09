pipeline {
  agent any
  tools { 
        maven 'Maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nvndntbuggywebapp -Dsonar.organization=nvndntbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b05efde82cc9166d98b4bd90473f9226b685db36'
			}
        } 
  }
}
