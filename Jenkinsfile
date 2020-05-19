pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        bat(script: 'https://github.com/innomatics321/java-tomcat-maven-example.git', encoding: 'master', label: 'java tomcat')
      }
    }

    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }

  }
}