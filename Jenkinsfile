
pipeline{
  agent any
  
  tools{
  }
  
  stages{
                stage("run frontend"){
                  steps{
                          echo 'executing yarn'
                          nodejs('Node-10.17'){
                              sh 'yarn install'
                          }
                      }
                   }
    
                stage("run backend"){
                  steps{
                          echo 'executing gradle'
                          withGradle('Gradle-6.2'){
                              sh './gradle -v'
                          }
                      }
                   }
    }
}
