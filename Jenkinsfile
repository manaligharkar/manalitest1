pipeline {
   agent any

   stages {
      stage('input statement') {
        options {
            timeout(time:2, unit: 'HOURS')
         }
         steps {
            input message: 'DONE??'
         }
         post {
            success {
               echo "App started successfully :)"
            }
            aborted {
               echo "App failed to start :( OMG"
            } 
            }
            }
       stage(' last') {    
        steps {
            echo "$GIT_BRANCH"
            echo "$GIT_COMMIT"
         }
      }
      }
      }
