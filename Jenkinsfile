
pipeline{
agent any
options{

skipDefaultCheckout(true)
     
}

stages {

     stage("SCM checkout")
     {
     steps{
       cleanWs()
       checkout scm

     }
     }

    stage("build")
    {
    steps{
       
       sh 'mvn clean install'

    }

   }

}



}
