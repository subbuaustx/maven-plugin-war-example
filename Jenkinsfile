pipeline {
   agent any

   tools {
      // Install the Maven version configured as "M3" and add it to the path.
      maven "Maven"
   }

   stages {
      stage('Build') {
         steps {
       
            bat "mvn -Dmaven.test.failure.ignore=true clean package"

         }

         post {
            success {
               echo 'Hello God'
            }
         }
      }
   }
}
