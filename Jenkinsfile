pipeline{
  agent any 
  stages{
    stage("checkout"){
      steps{
        checkout scm 
      }
    }
    stage("Test"){
          steps{
            sh 'sudo apt install npm -S '
            sh 'npm test'
          }
    }
    stage("Build"){
      steps{
        sh 'npm run build'
      }
    }
  }
}
