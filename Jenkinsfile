 def workspace;
node{
   stage ('Checkout')
   {
       
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '1d63b82f-52b3-412d-951e-9029e47d7382', url: 'https://github.com/bibek0914/amazon.git']]])
       workspace=pwd()
   }
    stage('static code analysis')
   {
     echo ("static code analysis")
   }
   stage('Build')
   {
     echo ("Build the code")
}
stage('testing')
   {
     echo ("testing")
}
stage('Delivary')
   {
     echo ("delivary")
}
}
