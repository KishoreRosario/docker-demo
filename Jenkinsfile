pipeline {
  environment {
    imageName = "kishorerosario/my-first-jenkins-docker"
    registryCredential = 'dockerhub'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/KishoreRosario/docker-demo.git', branch: 'master'])
      }
    
    stage('Building image') {
 	    steps {
 	      script {
 	        dockerImage = docker.build imagename
 	      }
 	    }
 	  }
      
  }
  
}
