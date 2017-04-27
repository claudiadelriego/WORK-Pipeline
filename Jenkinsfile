#!groovy

node{
   checkout scm
   }

pipeline {
agent any

   stages {

   stage ('Build0'){
     steps{
        sh 'ls -la'
     }
   }
   stage ('Build1'){
     steps{
        sh 'mvn -Dtest=SampleTest2 test'
     }

   }

    stage ('Build'){
      steps{
          sh 'make'
          junit '**/surefire-reports/*.xml'
      }
    }
  }









}


