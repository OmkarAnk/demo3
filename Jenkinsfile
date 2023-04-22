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
    sh 'sudo docker build /home/ubuntu/.jenkins/workspace/assign1 -t web'
    sh 'sudo docker run --name myweb -d -88:80 web'
  }
  
}
