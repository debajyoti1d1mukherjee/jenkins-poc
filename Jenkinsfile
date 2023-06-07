pipeline {
  agent any
  stages {
    stage('for master branch') {
      when {
        branch 'master'
      }
      steps {
        echo 'master branch'
      }
    }
    stage('for production branch') {
      when {
        branch 'production'
      }
      steps {
        echo 'production branch'
      }
    }
    stage('for pull request') {
      when {
        changeRequest()
      }
      steps {
        echo 'pull request'
      }
    }
  }
}