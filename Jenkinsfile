node('built-in')
{
  stage('Download')
  {
    git 'https://github.com/OmkarAnk/demo3.git'
  }
  stage('Build')
  {
    sh '''
            # Get container IDs
            container_ids=$(sudo docker ps -aq)
            
            # Check if there are any containers
            if [ -n "$container_ids" ]; then
                # Remove containers
                sudo docker rm -f $container_ids
            else
                echo "No containers to remove."
            fi
        '''
  }
  
}
