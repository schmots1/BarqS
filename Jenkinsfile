pipeline {
  agent {
    docker {
      image 'ubuntu'
    }
    
  }
  stages {
    stage('pull code') {
      steps {
        git(url: 'https://github.com/schmots1/Excel-mysql.git', branch: 'master')
      }
    }
    stage('script') {
      steps {
        sh 'ls'
      }
    }
  }
  environment {
    name = 'image'
  }
}