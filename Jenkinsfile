pipeline {
    agent any
  
    stages {
        stage ('Complile Stage') {
            steps {
               withMaven(maven : 'maven_3_1_1')
                    sh 'mvn clean compile'
                }
            }
         stage ('Build Stage') {
            steps {
               withMaven(maven : 'maven_3_1_1')
                    sh 'mvn clean test'
                }
            }
          stage ('Deployment Stage') {
            steps {
               withMaven(maven : 'maven_3_1_1')
                    sh 'mvn clean deploy'
            }
        }
      
    }
}
