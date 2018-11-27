pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout scm
        script {
                def content = readFile 'gradle.properties'
                echo "${content}"
                }
        }
    }
  }
}
