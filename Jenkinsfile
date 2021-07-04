pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Placeholder'
        sh './jenkins/build.sh'
      }
    }

    stage('Test') {
      steps {
        sh 'sleep 5'
        sh 'echo Success!'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Placeholder'
      }
    }

  }
  environment {
    MYVAR = 'Madanraj'
  }
}