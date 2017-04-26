#!groovy

node{

stage 'checkout'
    git url: 'https://github.com/claudiadelriego/WORK-Pipeline.git'


stage 'Build'
   echo 'DONE'

stage 'Build2'
sh 'mvn test'
sh step([$class: 'JUnitResultArchiver', testResults: '**/target/surefire-reports/TEST-*.xml'])

}