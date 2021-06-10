pipeline{
  agent any
  stages{
    stage('Example Build'){
      steps{
        sh 'mvn clean install'
        sh 'cd target/' 
        sh 'ls -la' 
        def myFile = new File("target/demo-0.0.1-SNAPSHOT.jar")
        build (job : 'Folder/Deploy on Ontwikkel', wait : false, propagate : false, parameters : [
          string(name :'HELLO', value : 'Jasper Fennet'), 
          file(name : 'artifact', file : myFile)
               ])
        echo 'Deploy Job started'
      }
    }
  }

}
