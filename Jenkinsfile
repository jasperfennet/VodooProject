pipeline{
  agent any
  stages{
    stage('Example Build'){
      steps{
        echo 'helllo'
        build (job : 'Folder/Deploy on Ontwikkel', parameters : [string('name', 'jasper')])
        echo 'Deploy Job started'
      }
    }
  }

}
