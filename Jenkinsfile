pipeline {
  agent { label "slave1" }
  environment {
    gradleHome = tool 'gradle4'
  }
  stages {
    stage('checkout') {
      steps {
        checkout scm
      }
    }
    stage('build') {
      steps{
        sh "${env.gradleHome}/bin/gradle build"
      }
    }
  }
}
