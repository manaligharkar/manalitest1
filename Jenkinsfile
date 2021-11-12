pipeline {
   agent any

   stages {
      stage('input statement') {
        input {
                message 'Deploy?'
                ok 'Do it!'
               }
         steps {
            echo 'DONE'
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
