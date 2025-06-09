pipeline{
  agent any
  tools{
    gradle 'Gradle'
    jdk 'JDK'
  }
  stages{
    stage('checkout'){
      steps{
        git branch:'master',url:'https://github.com/Yoganand30/Mygradleprac.git'
      }
    }
  stage('build'){
    steps{
      sh './gradlew build'
    }
  }
  stage('test'){
    steps{
      sh './gradlew test'
    }
  }
    stage('run'){
      steps{
        sh './gradlew run'
      }
    }
  }
}
