pipeline{
  agent any
  stages{
    stage("checkout"){
      steps{
            git branch: 'feature', credentialsId: '286e0c4f-cfec-4072-b69b-295c0668eda9', url: 'https://github.com/kushahcl/A001.git'     
}
    } 
    stages{
      stage("Build"){
        steps{
        sh 'mvn clean compile'
        }
      }
    }
        stages{
      stage("test"){
        steps{
        sh 'mvn clean Test'
        }
      }
    }
     stages{
      stage("deploye"){
        steps{
        sh 'mvn clean package'
        }
      }
    }
  }      
 
}
