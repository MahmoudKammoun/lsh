pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/lsh/tree/master/src.git'
      }
    }
    stage('Compile') {
      steps {
        
        sh label: '', script: 'gcc -o lsh main.c'
      }
    }
  }
}
