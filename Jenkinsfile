pipeline {
  agent any 
  stages {
    stage ('Initialize') {
      steps {
        sh '''
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
            ''' 
      }
    }
    stage ('Generate build') {
      steps {
        sh 'mvn clean install -DskipTests'
      }
    }
  } 
}
