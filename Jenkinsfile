pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/lsh.git'
      }
    }
    
    stage('Configure the Linux kernel features and modules') {
      steps {
         sh label: '', script: 'cp -v /boot/config-$(uname -r) .config'
      }
    }
  }
}
