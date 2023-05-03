@Library('robot-shared-library')
pipeline 
{
 agent any
 stages 
 {
    stage ('lint checks') 
        {
     steps 
     {
      script{
          sample.info("Starting","DevOps.com")
      }
       sh "echo installing JSLINT"
       sh "npm install jslint"
       sh "ls -ltr node_modules/jslint/bin"
       // sh "./node_modules/jslint/bin/jslint.js server.js"
       sh "echo LINT CHECKS COMPLETED !!!"
     }
    }
    stage ('downloading the dependencies')
     {
      steps 
      {
        sh "npm install"
      }

    }
 }
}