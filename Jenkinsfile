pipeline {

  agent any

  parameters {
    string(name: 'COMPONENT', defaultValue: '', description: 'Component')
    string(name: 'APP_VERSION', defaultValue: '', description: 'App Version')
  }

  stages {

    stage('Get Values file') {
      steps {
        dir('APP') {
          git branch: 'main', url: 'https://github.com/raghudevopsb70/${COMPONENT}.git'
        }
      }
    }

    stage('Helm Deploy') {
      steps {
        sh 'find .'
      }

    }


  }

}