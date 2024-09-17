pipeline {
  agent any
  stages {
    stage('pull code from git') {
      steps {
        git(url: 'https://github.com/sudhirchaudhary08/test.git', branch: 'main')
      }
    }

    stage('install apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('deploy app') {
      steps {
        sh 'sudo cp -R * /var/www/html'
      }
    }

  }
}