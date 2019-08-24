pipeline{
agent any
stages{
stage('BUILD'){
steps
{
withMaven(maven : 'MVN3.3.9')
{
sh 'mvn clean compile'
}
}
}


stage('TEST'){
steps
{
withMaven(maven : 'MVN3.3.9')
{
sh 'mvn test'
}
}
}

stage('DEPLOY'){
steps
{
withMaven(maven : 'MVN3.3.9')
{
sh 'mvn deploy'
}
}
}

}
}