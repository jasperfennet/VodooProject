pipeline{
  agent any
  stages{
    stage('Example Build'){
      steps{
        echo 'helllo'
        build (job : 'Folder/Deploy on Ontwikkel', wait : false, propagate : false, parameters : [string(name :'name', value : 'Jasper Fennet')])
        echo 'Deploy Job started'
      }
    }
  }

}
