node{
   // Configure branch
   git branch: 'development', credentialsId: 'jenkins_deploy', url: 'git@github.com:mafitconsulting/mafitlabsrepo.git'
  
   //Set the Jenkins credentials that hold out Puppet Enterprise RBAC token 
   puppet.credentials 'jenkins_deploy'

   stage 'Deploy to dev'
   puppet.codeDeploy 'development'
}
       
