pipeline{
  agent any
  stages{
    stage('Example Build'){
      steps{
        sh 'mvn clean install'
        sh 'cd target/' 
        sh 'ls -la' 
        build (job : 'Folder/Deploy on Ontwikkel', wait : false, propagate : false, parameters : [
          string(name :'HELLO', value : 'Jasper Fennet'), 
          file(name : 'artifact', file : "demo-0.0.1-SNAPSHOT.jar")
               ])
        echo 'Deploy Job started'
      }
    }
  }

}
