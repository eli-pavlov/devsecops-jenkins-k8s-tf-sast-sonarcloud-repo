pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=elibuggywebapp_test -Dsonar.organization=elibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=44887f4fc985125761c1c3f0db96c3706e27a270'
			}
        } 
  }
}
