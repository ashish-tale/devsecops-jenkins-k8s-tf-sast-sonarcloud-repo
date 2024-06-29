pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jenkins_tf -Dsonar.organization=jenkins_tf -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fc30d2ca450588d80fc730c8f7f54a17b05ff9799'
			}
        } 
  }
}
