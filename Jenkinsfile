pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        git(url: 'https://github.com/innomatics321/Narendraapplication.git', branch: 'master', credentialsId: 'innomatics321')
      }
    }

    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }

    stage('deploy') {
      steps {
        bat 'xcopy "C:\\Program Files (x86)\\Jenkins\\workspace\\java tomcat\\target" "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps"/y'
      }
    }

  }
}