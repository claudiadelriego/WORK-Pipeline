#!groovy
pipeline {

   node {
       checkout scm
    }

   agent any

   stages {

    stage ('Build'){
      steps{
          sh 'make'
          archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
      }
    }
  }









}

stage 'Build2'
 sh 'mvn -Dtest=SampleTest2 test'
