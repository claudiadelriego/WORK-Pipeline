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

    stage ('Build'){
      steps{
          sh 'make check || true'
          junit '**/surefire-report/*.xml'
      }
    }
  }









}


