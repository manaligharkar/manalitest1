pipeline {
   agent any

   stages {
      stage('input statement') {
        input {
                message 'Deploy?'
                ok 'Do it!'
                
            }
        post {
            success {
               echo "App started successfully :)"
            }
            failure {
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
