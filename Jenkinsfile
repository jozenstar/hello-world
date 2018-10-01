pipeline {
  agent any 

  stages {
    
    stage('Say Hello!'){
     steps { echo "Hello from feature-1 branch" }
    }
  }
  post{
    success {
     mail to: 'artour.yazhevich@gmail.com',
     subject: "Pipeline ${currentBuild.fullDisplayName} works!",
     body: "${env.BUILD_URL} has succeeded"
     } 
  }
}

