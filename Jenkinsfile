pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh """
               echo "Building Artifact"
               """
           }
       }
	   stage('Test Code') {
          steps {
               sh """
               echo "Deploying Code"
			   cd /var/jenkins_home/workspace/Multibranch_Job1_TESTMULTI_BR
			   bash test.sh
               """
          }
      }
      stage('Deploy Code') {
          steps {
               sh """
               echo "Deploying Code"
               """
          }
      }
   }
}
