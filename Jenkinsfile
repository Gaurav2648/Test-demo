pipeline{
    
    agent any 
    
    stages {
        stage('build') {
            steps {
               script {
                   //Ensure Maven is in path
                   bat 'mvn -v' //verify maven installation
                   bat ' mvn clean install' //run the maven build
               }
            }
        }
        stage('package') {
            steps {
                script {
                      bat 'docker build .'   
                
            }
        }
    }
}
