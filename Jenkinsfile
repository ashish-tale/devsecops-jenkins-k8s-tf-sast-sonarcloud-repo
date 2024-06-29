pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonar0 -Dsonar.organization=sonar0 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=64a1be453f1ec70f46f8a2d8db7bbf931eee1177'
			}
        } 
  }
}
