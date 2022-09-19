pipeline {
  agent any
  stages {
    stage('git clone and cd') {
      steps {
        sh 'if [ -d "$WORKING_DIR" ]; then rm -Rf $WORKING_DIR; fi && git clone https://github.com/bro-da/django-dockersample && cd django-dockersample '
      }
    }

    stage('docker build') {
      steps {
        sh 'sudo docker-compose run web django-admin startproject composeexample .'
      }
    }

  }
}