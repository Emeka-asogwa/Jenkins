pipeline {
  agent any 
    tools {
        maven "myMaven"
    }
  
  stages{
  	stage('Build') {
      steps{
        // sh 'mvn --version'
		    echo "Build"
      }
	  }
	  stage('Test') {
      steps{
		    echo "Test"
      }
	  }
    stage("Integration Test"){
      steps{
        echo "Integration test "
      }
    }
  } 
  post {
    always {
      echo "I am great, Menco"
    }
    success {
      echo "Success!"
    }
  }
}