pipeline {
    
    agent any
    stages {
        stage ('initialize') {
            steps {
                bat 'mvn clean package'

                /*for Mac & Linux machine */
                // sh 'mvn clean package'
                
                }
        }
            post{
                success{
                  echo 'Now Archiving'
                  //achiveArtifacts artifacts : '**/*.war'
            }

        }
    }
}