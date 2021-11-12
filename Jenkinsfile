pipeline {
   agent any

   stages {
      stage('when statement') {
        when {
          branch 'master'
          }
        steps {
            input message: "Shall we Deploy?"
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
