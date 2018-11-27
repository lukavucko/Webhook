pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout scm
        script {
              //  def content = readFile 'gradle.properties'
              def props = readProperties file:'gradle.properties'
              def var1 = props['version']
                echo "${var1}"
                }
        }
    }
  }
}
