node('puppetmaster-slave') {
   // Configure branch
   git branch: 'development', credentialsId: 'deploy', url: 'git@github.com:mafitconsulting/mafitlabsrepo.git'
  
   //Set the Jenkins credentials that hold out Puppet Enterprise RBAC token 
   puppet.credentials 'deploy'

   stage 'Deploy to dev'
   puppet.codeDeploy 'development'
   puppet.job 'development'

}
       
