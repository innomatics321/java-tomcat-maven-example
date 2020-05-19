pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        bat 'https://github.com/innomatics321/java-tomcat-maven-example.git'
      }
    }

    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }

  }
}