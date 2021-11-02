pipeline {
  agent any

  tools {
    gradle 'gradle'
  }
  stages {
    stage('Build') {
      steps {
        git(
          url: "https://github.com/tomasmoreira04/is-ci",
          branch: "master",
          credentialsId: "tp-is"
        )
        sh 'chmod +x gradlew'
        sh './gradlew init'
        sh './gradlew spotlessApply'
        sh './gradlew build'
      }
    }
    stage('Test') {
      steps {
        echo 'dummy'
      }
    }
    stage('Validate') {
      steps {
        echo 'dummy'
      }
    }
    stage('Deploy') {
      steps {
        echo 'dummy'
      }
    }
  }
}
