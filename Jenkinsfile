pipeline {
      agent any
        stages {
            stage ('Compile Stage'){
              steps {
                withMaven(maven: 'Maven_3_6_3') {
                  sh 'mvn clean compile'
            }
         }
      } 
      stage ('Testing Stage'){
          steps {
              withMaven(maven: 'Maven_3_6_3') {
      sh 'mvn Test'
          }
       }
    } 
    stage ('Deployment Stage'){
      steps {
        withMaven(maven: 'Maven_3_6_3') {
            sh 'mvn Deploy'
              }
           }
        } 
      }
  } 
