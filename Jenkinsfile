pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-aws-app -Dsonar.organization=devsecops-aws-app -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fc8013749f7b6bb144f291f650e6b0fcaa6c5791'
			}
        } 
  }
}
