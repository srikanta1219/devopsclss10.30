pipeline {
   agent any
   tools {
     maven "maven"  
   }
   stages {
      stage('Git Checkout') {
         steps {
            git ''https://github.com/srikanta1219/devopsclss10.30.git'   
         }
      }
    
    stage ('Maven Goal'){
      steps {
         sh "mvn clean install package    " 
      }    
    }
 }
     post {
        always {
          cleanWs()
        }
    }
}
