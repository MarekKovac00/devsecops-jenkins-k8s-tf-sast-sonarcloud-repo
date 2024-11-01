pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=DP-MK-ORG -Dsonar.organization=buggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a376a9599040cf78007e0e157a2876ca960a33cc'
			}
        } 
  }
}
