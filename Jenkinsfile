pipeline {
agent any
stages {
stage('Fetch File') {
steps { git branch: 'main', url: 'https://github.com/Anjali-sahu830/jenkins-java-demo.git'
}
}
stage('Building') {
steps {
echo 'Building Project....'
bat 'javac Hello.java'
}
}
stage('Execution') {
steps {
echo 'Executing Program'
bat 'java Hello'
}
}
stage('Deploy') {
steps {
echo 'Deploying....'
}
}
}
post{
success{
echo 'PipeLine Executed Successfully'
}
failure{
echo 'PipeLine Failed'}}}
