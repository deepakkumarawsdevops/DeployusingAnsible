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
       mvn package
       mvn install
  } 

  } 

   stage('')
 {
  steps
  {
    echo 'Deployment'
  }

  }



}


} 
