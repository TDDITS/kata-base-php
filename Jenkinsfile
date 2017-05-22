pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '/usr/bin/composer install'
      }
    }
    stage('Test') {
      steps {
        sh './vendor/bin/phpunit test'
      }
    }
  }
}