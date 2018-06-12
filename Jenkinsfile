pipeline {
  agent any
  tools{
 	maven 'LocalMaven'
        jdk 'LocalJDK8'
      }
  stages{
     stage('Build KPApi'){
	steps{
           echo "----------------Building KPApi---------------------"
	   cd KPApi/
           mvn clean install -Dmaven.test.skip=true
	   echo "---------------KPApi Build is Success--------------"
	  }
       }
   }
}
