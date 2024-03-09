pipeline{
  agent any
  stages{
    stage('Build'){
steps{
build 'PES1UG22CS842-1'
sh 'g++ main/file2.cpp -o output'
}
}
stage('Test'){
steps{
sh './output'
}
}
stage('Deploy'){
steps{
echo 'deploy'
}
}
}
post{
failure{
error 'pipline failed'
}
}
}
