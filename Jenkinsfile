pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/lsh.git'
      }
    }
    stage('dep') {
      steps {
        
        sh label: '', script: 'cd src'
      }
    }
    stage('Compile') {
      steps {
        
        sh label: '', script: 'gcc main.c'
      }
    }
  }
}
