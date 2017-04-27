#!groovy
pipeline {

   agent any

   stages {

   stage ('Checkout'){
    checkout scm
   }

    stage ('Build'){
      steps{
          sh 'make'
          archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
      }
    }
  }









}


