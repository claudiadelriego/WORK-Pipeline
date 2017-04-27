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
        sh 'mvn -Dtest=SampleTest2 ${target}'
     }

   }

    stage ('Build'){
      steps{
         echo "Ambiente: ${env.BUILD_ID} on ${env.JENKINS_URL}"
      }
    }
  }









}


