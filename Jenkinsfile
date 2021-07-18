pipeline {
  agent any
  stages {
    stage('PreBuild') {
      steps {
        echo 'POM Validation'
        sh 'sh run prebuild.sh'
      }
    }

    stage('SonarJob') {
      steps {
        echo 'SonarJob'
        sh 'sh run sonarjob.sh'
      }
    }

    stage('Build') {
      steps {
        echo 'Buuiling the war file'
        sh 'sh run buildjob.sh'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy on server'
        sh 'sh run deployjob.sh'
      }
    }

  }
}