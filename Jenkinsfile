#!groovy
pipeline {

   agent any

   stages {

   stage ('Build0'){
   node{
    checkout scm
    }
   }

    stage ('Build'){
      steps{
          sh 'make'
          archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
      }
    }
  }









}


