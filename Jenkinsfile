node {
   // Configure branch
   git branch: 'development', credentialsId: 'deploy', url: 'git@github.com:mafitconsulting/mafitlabsrepo.git'
  
   //Set the Jenkins credentials that hold out Puppet Enterprise RBAC token 
   puppet.credentials 'deploy'

   // Deploy enviornment to Dev
   //stage ('Deploy to development') {
   //  lock(‘puppet-code-development’) {
   //    puppet.codeDeploy 'development'
   //    puppet.job 'development', nodes: ['fieldhousem3.mylabserver.com','puppetagent']
   //  }
   //}
   stage 'Deploy to dev'
   puppet.codeDeploy 'development'
   puppet.job 'development'

}
       
