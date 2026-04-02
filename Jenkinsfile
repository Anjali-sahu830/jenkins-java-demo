pipeline {
agent any
stages {
stage('Checkout') {
steps {
  git branch: 'main', url: 'https://github.com/Anjali-sahu830/jenkins-java-demo.git'
}
}
stage('Publish') {
steps {
publishImage([
  allowMissing:true,
  alwaysLinkToLastBuild:false,
  keepAll:false,
  reportDir:'.',
  reportFiles:'html1.html',
  reportName:'My html publish'
])
  }
}
}}

    
