pipeline {
  agent any
  stages {
    stage('check tools') {
      steps {
        sh '''mvn --version
git --version
java -version'''
      }
    }

    stage('build') {
      steps {
        sh 'mvn compile test package'
      }
    }

    stage('deploy') {
      steps {
        echo 'deployment stage'
      }
    }

  }
}