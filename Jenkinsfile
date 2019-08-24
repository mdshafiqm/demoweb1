pipeline{
agent any
stages{
stage('BUILD step'){
steps
{
withMaven(maven : 'maven')
{
sh 'mvn clean compile'
}
}
}


stage('TEST'){
steps
{
withMaven(maven : 'maven')
{
sh 'mvn test'
}
}
}

stage('DEPLOY'){
steps
{
{
input(Do you want to proceed)
{
withMaven(maven : 'maven')
{
sh 'mvn deploy'
}
}
}

}
}