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
        build 'Folder/Deploy on Ontwikkel'
        echo 'Deploy Job started'
      }
    }
  }

}
