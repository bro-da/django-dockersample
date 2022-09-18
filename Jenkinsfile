pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        git(url: 'https://github.com/bro-da/django-dockersample', branch: 'master')
      }
    }

    stage('source venv') {
      steps {
        sh 'cd django-dockersample && python3 -m venv venv && source venv/bin/activate'
      }
    }

  }
}