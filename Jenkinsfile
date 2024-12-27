pipeline {
  agent any
  stages{
    stage("Maven Build"){
      when {
        branch "develop"
      }
      steps{
        echo "Hello this is maven build"
      }
    }
        stage("Test Deploy"){
      when {
        branch "test"
      }
      steps{
        echo "deploy to test...."
      }
    }
     stage("Prod Deploy"){
      when {
        branch "main"
      }
      steps{
        echo "deploy to production...."
      }
    }
    
  }
}
