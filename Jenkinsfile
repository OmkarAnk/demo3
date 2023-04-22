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
    sh 'sudo docker rm -f $(sudo docker ps -aq)'
    sh 'sudo docker system prune -af'
    sh 'sudo docker build /home/ubuntu/.jenkins/workspace/assign1 -t web'
    sh 'sudo docker run -d -P web'
    sh 'sudo docker ps'
  }
  
}
