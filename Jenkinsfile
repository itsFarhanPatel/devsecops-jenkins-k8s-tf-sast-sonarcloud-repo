pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopspro -Dsonar.organization=devsecopspro -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f2231fcf04eed033c79c9ce9c7b6e944756bfb05'
			}
        } 
  }
}
