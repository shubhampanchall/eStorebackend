pipeline{
agent any
stages{
stage('Source'){
steps{
git branch:'main',url:'https://github.com/shubhampanchall/eStorebackend.git'
}
}
stage('Compile'){
steps{
bat "./mvnw compile"
}
}
stage('Test'){
steps{
bat "./mvnw test"
}
}
stage('Build'){
steps{
bat "./mvnw package"
}
}
}
}
