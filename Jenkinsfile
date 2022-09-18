pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/bro-da/django-dockersample', branch: 'master')
        sh 'cd django-dockersample'
      }
    }

  }
}