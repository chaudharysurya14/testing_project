pipeline {
  agent any 
    stage ('Generate build') {
      steps {
        sh 'mvn clean install -DskipTests'
     }
  }  
}
