pipeline 
{
 agent any
 stages 
 {
    stage ('lint checks') 
    {
     steps 
     {
       sh "echo installing JSLINT"
       sh "npm install jslint"
       sh "ls -ltr node_modules/jslint/bin"
       sh "./node_modules/jslint/bin/jslint.js server.js"
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