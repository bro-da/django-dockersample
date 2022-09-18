pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/bro-da/django-dockersample', branch: 'master')
      }
    }

    stage('install dependecies') {
      steps {
        sh 'cd django-dockersample && pip install -r requirements.txt'
      }
    }

  }
}