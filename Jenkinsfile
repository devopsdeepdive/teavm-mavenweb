pipeline {
agent any
  //agent {
  //label 'jenkins_slave'
//}
  stages {
  stage('Checkout') {
    steps {
      checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_cred', url: 'https://github.com/devopsdeepdive/teavm-maven-webapp.git']])
    }
  }

}

}
