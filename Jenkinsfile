pipeline {
    agent any
  
    stages {
        stage ('Complile Stage') {
            steps {
               
                    sh 'mvn -f vasudata/pom.xml clean package'
                }
            }
         stage ('Build Stage') {
            steps {
               withMaven(maven : 'maven_3_1_1')
                    sh 'mvn -f vasudata/pom.xml clean test'
                }
            }
          stage ('Deployment Stage') {
            steps {
               withMaven(maven : 'maven_3_1_1')
                    sh 'mvn -f vasudata/pom.xml clean deploy'
            }
        }
      
    }
}
