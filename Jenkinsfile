pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=StephanoHerrera_devsecops-jenkins-k8s-tf-sast-sonarcloud-repo -Dsonar.organization=technicalwankery -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8d37d548ea876bdfd300eecf763013f5344774f5'
			}
        } 
  }
}
