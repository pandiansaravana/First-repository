pipeline {
  agent {
    node {
      label 'Linux-slave'
    }

  }
  stages {
    stage('Download source code') {
      steps {
        git 'https://github.com/apache/maven.git'
      }
    }
    stage('maven package') {
      steps {
        sh 'mvn package'
      }
    }
  }
}