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
                    sh 'mvn -f vasudata/pom.xml clean test'
                }
            }
          stage ('Deployment Stage') {
            steps {
                    sh 'mvn -f vasudata/pom.xml clean deploy'
            }
        }
      
    }
}
