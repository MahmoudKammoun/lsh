pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/lsh.git'
      }
    }
    
    stage('Compile') {
      steps {
         sh label: '', script: 'gcc -o lsh2 src/main.c'
      }
    }
  }
}
