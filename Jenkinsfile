// Jenkinsfile-SimpleSharedLibrary
// ----------------------------------------------------------------------
// Simple Jenkinsfile example showing how to call a shared library
// Important Note: The shared library is found in the var directory
//    in this repo and Jenkins needs to be configured to use the
//    library prior to executing this pipeline (see instructions
//    in the repo's readme)
// ----------------------------------------------------------------------

// Library this Jenkinsfile uses - configured in Manage Jenkins/Configure System
library 'lib'

pipeline {
   agent any
   stages {
      stage('Example') {
         steps {
         	// Call the getChangeset function
         	githubChangeset()
         	
            // Call the helloWorld() method and pass a value
            helloWorld("Craig")
         }
       }
   }
}
