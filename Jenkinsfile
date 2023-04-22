node('built-in')
{
  stage('Download')
  {
    git 'https://github.com/OmkarAnk/demo3.git'
  }
  stage('Build')
  {
    sh '''sudo docker ps -aq | xargs sudo docker rm -f'''
  }
  
}
