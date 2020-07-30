pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/MahmoudKammoun/lsh.git'
      }
    }
    
    stage('Compile') {
      steps {
         sh label: '', script: 'gcc -DLSH_USE_STD_GETLINE -o lsh3 src/main.c'
      }
    }
    stage('archive') {
      steps {
         sh label: '', script: 'tar -cvf lsh.tar lsh3'
      }
    }
  }
}
