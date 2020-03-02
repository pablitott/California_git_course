pipeline {
  agent any
  stages {
    stage('Build our website') {
      steps {
        sh 'whoami'
	sh 'pwd' 
        sh "scripts/build.sh"
      }
    }

    stage('Run unit tests') {
      steps {
        sh 'whoami'
        sh 'pwd'
        echo "I'm in unit tests"
        sh "scripts/unit_tests.sh"
      }
    }

    stage('Deploy website') {
      steps {
        sh 'whoami'
        sh 'pwd'
        echo "Deploy website"
        sh "scripts/deploy_website.sh"
      }
    }
  }
}
