pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git source: 'https://github.com/RandriamihajaOlivierMartial/Test.git', branch: 'main', credentialsId: '569a8f7c-cd24-4238-ad9c-903648847aaa'
      }
    }
    stage('Build'){
      steps{
        // Assuming java is in the system path
        bat 'java HelloWord.java'

        // If java is not in the path, specify the full path
        // bat 'C:\path\to\java.exe MoneyBag.java'
      }
    }
    stage('Test'){
      steps{
        //bat 'java AllTest.java'
      }
    }
  }
}
