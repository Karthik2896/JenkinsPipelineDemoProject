pipeline{
agent any
stages 
{
stage('Build') 
{
steps{
echo "Building the Code.........."
withMaven(maven: 'maven-3.3.3') {
sh "mvn clean"
}
}
}
stage('Test') 
{
steps{
echo "Testing the Code.........."
sh "mvn test"
}
}
stage('Compile') 
{
steps{
echo "Compiling the Project.........."
sh "mvn compile"
}
}
}
}
