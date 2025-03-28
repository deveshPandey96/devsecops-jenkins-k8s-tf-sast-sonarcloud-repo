pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=initiallearning -Dsonar.organization=initiallearning -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e09981f859588c97f33cc9697d441b2564d3d696'
			}
        } 
  }
}
