pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout scm
        script {
                def content = readFile 'gradle.properties'
                PROP_KEY=$1
                PROP_VALUE=`cat $content | grep "$PROP_KEY" | cut -d'=' -f2`
                echo "${PROP_VALUE}"
                }
        }
    }
  }
}
