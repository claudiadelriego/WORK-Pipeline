#!groovy

node{
   checkout scm
   }

pipeline {
agent any


   stages {

   stage ('Build0'){
   sh 'ls -la'
   }

    stage ('Build'){
      steps{
          sh 'make'
          archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
      }
    }
  }









}


