pipeline {
agent any
stages {
  stage('Checkout') {
    steps {
      checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-user', url: 'https://github.com/devopsdeepdive/teavm-maven-webapp.git']])
    }
  }
  stage('Build') {
    steps {
     sh 'mvn compile'
    }
  }
  // stage('Test') {
   // steps {
    // sh 'mvn test'
    //}
  //}
   stage('Package') {
    steps {
     sh 'mvn package'
    }
  }

}
}
