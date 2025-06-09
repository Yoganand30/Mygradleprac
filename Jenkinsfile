pipeline {
  agent any

  tools {
    gradle 'Gradle'
    jdk 'JDK'
  }

  stages {
    stage('checkout') {
      steps {
        git branch: 'master', url: 'https://github.com/Yoganand30/Mygradleprac.git'
      }
    }

    stage('build') {
      steps {
        sh 'gradle build'
      }
    }

    stage('test') {
      steps {
        sh 'gradle test'
      }
    }

    stage('run') {
      steps {
        sh 'gradle run'
      }
    }
  }
}
