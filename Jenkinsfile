pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building'
        sh 'jenkins/build.sh'
        echo $?
      }
    }

    stage('test') {
      steps {
        echo 'Testing'
        sh 'jenkins/test.sh'
        echo $?
      }
    }

    stage('deploy') {
      steps {
        echo 'Deploying'
        sh 'jenkins/deploy.sh'
        echo $?
      }
    }

  }
}
