#!groovy
pipeline {

   agent any

   stages {

   stage ('Build0'){
   agent any
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


