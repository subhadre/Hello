pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
    stage("initilize build"){
      steps{
        sh '''
        echo "PATH=$PATH"
        echo "MAVEN=$MAVEN"
        '''
      }
      stage("Build"){
        steps{
          sh 'mvn clean package'
        }
      }
    }
  }
}
