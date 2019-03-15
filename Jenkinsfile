pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('Build') {
      steps {
        sh 'npm run build'
      }
    }
    stage('test') {
      steps {
        sh 'npm test'
        emailext(subject: 'onibi', body: 'hbhbbjbhb', attachLog: true, to: 'Jacg')
      }
    }
  }
}