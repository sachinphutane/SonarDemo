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

bat 'mvn sonar:sonar'

}
}
}
}
