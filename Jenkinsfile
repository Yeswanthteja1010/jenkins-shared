@Library('jenkins-shared-lib') _

pipeline {
  agent any

  stages {
    stage('Clone Repository') {
      steps {
        git url: 'https://github.com/Yeswanthteja1010/jenkins-shared.git', branch: 'main'
      }
    }

    stage('Build') {
      steps {
        sh 'echo "Building the application"'
      }
    }

    stage('Running Shared Library') {
      steps {
        script {
          commonBuild() 
        }
      }
    }
  }
}
