pipeline{
    
    agent any 
    
    stages {
        stage('build') {
            steps {
               scrpit {
                   //Ensure Maven is in path
                   bat 'mvn -v' //verify maven installation
                   bat ' mvn clean install' //run the maven build
               }
            }
        }
        stage('testing') {
             steps {
                 echo "my code is getting test..."
             }
        }
        stage('code anylaise') {
            steps {
                echo "my code is anyalise..."
            }
        }
        stage('deploy') {
            steps {
                echo "deploy my code..."
            }
        }
    }
}
