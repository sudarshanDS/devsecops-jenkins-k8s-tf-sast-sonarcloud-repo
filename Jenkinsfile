pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devopsbuggyapp -Dsonar.organization=devopsbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=77b509a99f0fff635e5fe25fc95fce2bb5b99e46'
			}
        } 
  }
}
