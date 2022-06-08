pipeline
{
agent any

stages
{
stage('Package')
{
steps
{
bat "mvn clean package"
}
}

stage('Sonar Analysis')
{
steps
{
 withSonarQubeEnv('SonarQube')
{
bat 'mvn sonar:sonar'
}
}
}
}
}
