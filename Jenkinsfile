pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Kebcombuggywebapp -Dsonar.organization=kebcombuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1de7c1d58826b4747299d98a5186a4ae24fb8a91'
			}
        } 
  }
}
