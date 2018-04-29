pipeline {
     agent any
     
     stages {
        stage ('Compile stage') {
          
          steps {
          
             withMaven(maven : 'maven-3.5') {
                sh 'mvn clean compile'
             }
          }
         
        }
        
        stage ('Test stage') {
          
          steps {
          
             withMaven(maven : 'maven-3.5') {
                sh 'mvn test'
             }
          }
         
        }
        
        stage ('Package stage') {
          
          steps {
          
             withMaven(maven : 'maven-3.5') {
                sh 'mvn package'
             }
          }
         
        }
     }
}
