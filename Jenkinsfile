pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=yashsedso -Dsonar.organization=yashsedso -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=76dc0ebfe32bab3709b70b6901654fed63e46658'
			}
        } 
  }
}
