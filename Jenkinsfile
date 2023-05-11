pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops -Dsonar.organization=yashse -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=24743267af19e114da79653f005b416bf6ac5ae9'
			}
        } 
  }
}
