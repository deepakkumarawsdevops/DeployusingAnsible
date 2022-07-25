pipeline
{ 
agent {label 'ansible-node'}

stages

{
 
 stage('Build WAR') 
 {
  steps
  {
       sh 'echo "Building" '
       sh 'mvn package'
       sh 'mvn install'
  } 

  } 

   stage('Deployment uisng Ansible')
 {
  steps
  {
    echo 'Deployment'

    sh 'ansible-playbook war-image.yml'
  }

  }



}


} 
