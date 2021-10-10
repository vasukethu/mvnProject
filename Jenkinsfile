pipeline {
    agent any
  
    stages {
        stage ('Complile Stage') {
            steps {
               
                    sh 'mvn -f MyNew_Pipe_Line_1/pom.xml clean package'
                }
            }
         stage ('Build Stage') {
            steps {
                    sh 'mvn -f MyNew_Pipe_Line_1/pom.xml clean test'
                }
            }
          stage ('Deployment Stage') {
            steps {
                    sh 'mvn -f MyNew_Pipe_Line_1/pom.xml clean deploy'
            }
        }
      
    }
}
