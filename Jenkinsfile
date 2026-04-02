pipeline {
agent any
stages {
stage('Checkout') {
steps {
  git branch: 'main', url: 'https://github.com/Anjali-sahu830/jenkins-java-demo.git'
}
}
stage('Build Image') {
steps {
bat 'docker build -t mywebsite .'
}
}
stage('Stop old container')
  {
steps {

bat 'docker stop mycont || exit 0'
bat 'docker rm mycont || exit 0'
}
}
stage('Run Image - Containerize'){
  steps{
    bat 'docker run -d -p 7000.80 --name mycont mywebsite'
  }
}
}}
    
