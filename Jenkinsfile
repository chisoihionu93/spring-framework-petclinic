import groovy.json.*

node () {
   def policyEvaluation

   stage('Preparation') {
      checkout scm
   }
    stage('Build') {
      // Run the maven build
            withMaven(maven: 'mvn3') {
            sh 'mvn clean install' 
            }
        }

         // sh 'chmod +x ./mvnw'
         // sh "./mvnw -Dmaven.test.failure.ignore -Dmaven.compiler.source=8 -Dmaven.compiler.target=8' clean install"
   }
}
