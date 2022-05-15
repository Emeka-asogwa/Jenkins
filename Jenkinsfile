pipeline {
  agent any
  // agent { docker { image 'node:13.8'}}
  stages{
  	stage('Build') {
      steps{
        sh 'mvn --version'
        sh 'docker version'
		    echo "Build"
        echo "$PATH"
        echo "BUILD_NUMBER - $env.BUILD_NUMBER"
        echo "$env.BUILD_ID"
        echo "$env.JOB_NAME"
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