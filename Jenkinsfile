pipeline {
    agent any 
    stages {
        stage('Compile Repository and Clean WorkSapce') { 
            steps {
               
                sh " mvn clean  compile"
            }
        }
        stage('Test') { 
            steps {
               sh " mvn test "
            }
        }
        stage('Deploy') { 
            steps {
                sh " mvn package "
            }
        }
    }
}
