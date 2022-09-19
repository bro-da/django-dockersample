pipeline {
  agent any
  stages {
    stage('git clone and cd') {
      steps {
        sh 'if [ -d  django-dockersample]; then rm -Rf django-dockersample; fi || git clone https://github.com/bro-da/django-dockersample && cd django-dockersample '
      }
    }

    stage('docker build') {
      steps {
        sh 'docker-compose run web django-admin startproject composeexample .'
      }
    }

  }
}