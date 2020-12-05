pipeline {
    agent { node { label 'Dev' } }
    stages{
        stage("Build") {
         steps {
          git credentialsId: 'ad1ecaac-1ea5-4b51-ab6a-5a038faf16a4', url: 'https://github.com/zainadnan/test'
         
          script {
           echo "moving"
           sh 'cd /var/www/html/ sudo cp /var/lib/jenkins/workspace/estpipelne-decl/index.html'    
          } 
         }
        }
        stage("Test"){
         steps {
          echo "123"
         }
        }
    }
}    
