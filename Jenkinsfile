pipeline{
  agent any
  stages{
    stage('Maven clean install'){
      steps{
        sh 'mvn clean install'
      }
    }
    stage('Example Build'){
      steps{
        echo 'helllo'
        build (job : 'Folder/Deploy on Ontwikkel', parameters : [string('name', 'jasper')])
        echo 'Deploy Job started'
      }
    }
  }

}
