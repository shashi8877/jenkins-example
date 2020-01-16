pipeline {
      agent any
        stages {
        stage ('Compile Stage'){
        steps {
        withMaven(maven : 'Maven_3_6_3') {
        sh 'mvn clean complile'
            }
         }
      } 
      stage ('Testing Stage'){
      steps {
      withMaven(maven : 'Maven_3_6_3') {
      sh 'mvn Testing'
          }
       }
    } 
    stage ('Testing Deploy'){
    steps {
    withMaven(maven : 'Maven_3_6_3') {
    sh 'mvn Deploying'
              }
           }
        } 
      }
  } 
