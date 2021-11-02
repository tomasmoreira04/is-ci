pipeline {
  agent any
  
  tools {
    gradle 'gradle'
  }
  stages {
    stage('Build') {
      steps {
        sh 'git pull https://github.com/sperdich/UTN.git'
        sh 'chmod +x gradlew'
        sh './gradlew init'
        sh './gradlew build'
      }
    }
    stage('Test') {}
    stage('Validate') {}
    stage('Deploy') {}
  }
}
