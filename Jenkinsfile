pipeline {
  agent {
    docker {
      args 'p 3000:3000'
      image 'openjdk:8-jdk-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sh \'mvn -B -DskipTests clean package\''
      }
    }

  }
}