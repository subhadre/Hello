pipeline {
  agent any 
  
  stages {
    stage ('Initialize') {
      steps {
        sh '''
              echo "M2_HOME = ${M2_HOME}"
            ''' 
      }
    }
    stage ('Build') {
      steps {
      sh 'mvn clean package'
       }
    }
            
  }
}
