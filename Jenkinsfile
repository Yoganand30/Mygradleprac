pipeline {
  agent any
  tools {
    jdk 'JDK'
  }
  stages {
    stage('Checkout') {
      steps {
        git branch: 'master', url: 'https://github.com/Yoganand30/Mygradleprac.git'
      }
    }
    stage('Build') {
      steps {
        sh 'chmod +x gradlew'       // Make the wrapper executable
        sh './gradlew build'
      }
    }
    stage('Test') {
      steps {
        sh './gradlew test'
      }
    }
    stage('Run') {
      steps {
        sh './gradlew run'
      }
    }
  }
}
