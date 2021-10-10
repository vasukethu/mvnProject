pipeline {
    agent any
  
    stages {
        stage ('Complile Stage') {
            steps {
               
                    sh 'mvn -f /var/lib/jenkins/workspace/MyNew_Pipe_Line_1/pom.xml clean package'
                }
            }
         stage ('Build Stage') {
            steps {
                    sh 'mvn -f /var/lib/jenkins/workspace/MyNew_Pipe_Line_1/pom.xml clean test'
                }
            }
          stage ('Deployment Stage') {
            steps {
                    sh 'mvn -f /var/lib/jenkins/workspace/MyNew_Pipe_Line_1/pom.xml clean deploy'
            }
        }
      
    }
}
