pipeline {
  agent { 
    docker { image 'maven:3.8.1-adoptopenjdk-11'}
  }
  stages{
  	stage('Build') {
      steps{
        sh 'mvn --version'
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