pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        git(url: 'https://github.com/innomatics321/java-tomcat-maven-example.git', branch: 'master', credentialsId: 'innomatics321')
      }
    }

    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }

  }
}