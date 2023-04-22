node('built-in')
{
  stage('Download')
  {
    git ''
  }
  stage('Build')
  {
    sh 'sudo docker rm -f $(docker ps -aq)'
  }
  
}
