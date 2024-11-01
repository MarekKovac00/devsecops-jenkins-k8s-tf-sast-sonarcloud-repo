pipeline {
  agent any
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp -Dsonar.organization=dp-mk-org -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a376a9599040cf78007e0e157a2876ca960a33cc'
			}
        } 
  }
}
