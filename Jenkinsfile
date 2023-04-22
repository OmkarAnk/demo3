node('built-in')
{
  stage('Download')
  {
    git 'https://github.com/OmkarAnk/demo3.git'
  }
  stage('list')
  {
    echo "Workspace: ${env.WORKSPACE}"
  }
  stage('Build')
  {
    sh 'sudo docker ps'
    sh 'sudo docker images'
  }
  
}
