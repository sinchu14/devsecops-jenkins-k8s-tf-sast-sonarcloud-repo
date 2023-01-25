pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopswebapp -Dsonar.organization=devsecopswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=547d44e8d9491afbb6a0fa8c4dbfc86977de7841'
			}
        } 
  }
}
