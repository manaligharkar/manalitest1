pipeline {
   agent any

   stages {
      stage('input statement') {
        options {
            timeout(time:1, unit: 'MINUTES')
         }
         steps {
            input message: 'DONE??'
         }
         post {
            success {
               echo "App started successfully :)"
            }
            aborted {
               echo "App failed to start :("
            } 
            }
            }
       stage(' last') {    
        steps {
            echo "$GIT_BRANCH"
         }
      }
      }
      }
