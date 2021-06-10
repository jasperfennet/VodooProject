pipeline{
  agent any
  stages{
    stage('Example Build'){
      steps{
        sh 'mvn clean install'
        sh 'cd target/' 
        sh 'ls -la' 
        build (job : 'Folder/Deploy on Ontwikkel', wait : false, propagate : false, parameters : [string(name :'HELLO', value : 'Jasper Fennet')])
        echo 'Deploy Job started'
      }
    }
  }

}
