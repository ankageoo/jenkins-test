pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building'
        sh 'jenkins/build.sh'
      }
    }

    stage('test') {
      steps {
        echo 'Testing'
        sh 'jenkins/test.sh'
      }
    }

    stage('deploy') {
      steps {
        echo 'Deploying'
        sh 'jenkins/deploy.sh'
      }
    }

  }
}