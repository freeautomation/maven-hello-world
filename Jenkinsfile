pipeline {
  agent any
  tools{
 	maven 'LocalMaven'
        jdk 'LocalJDK8'
      }
  stages{
     stage('Build KPApi'){
	steps{
          sh '''
           cd my-app
           echo "----------------Building KPApi---------------------"
           mvn clean install -Dmaven.test.skip=true
	   echo "---------------KPApi Build is Success--------------"
	  '''
	  }
       }
   }
}
