pipeline{

  agent any

  tools{
    maven 'Maven363'
  }

  stages{

    stage('build'){
      steps{
        sh 'mvn compile'
      }
    }

    stage('test'){
      steps{
        sh 'mvn clean test'
      }
    }

    stage('package'){
      steps{
        sh 'mvn package -DskipTests'
      }
    }

  }

}
