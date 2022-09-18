pipeline {
  agent any
  stages {
    stage('rebuilding docker directory') {
      steps {
        sh '''if [ -d /home/dev/temp/django-dockersample ]; then rm -Rf /home/dev/temp/django-dockersample; fi

 

  '''
        sh 'cd temp '
      }
    }

    stage('') {
      steps {
        git(url: 'https://github.com/bro-da/django-dockersample', branch: 'master')
      }
    }

    stage('py venv') {
      steps {
        sh '''python3 -m venv venv


| source venv/bin/activate'''
      }
    }

  }
}