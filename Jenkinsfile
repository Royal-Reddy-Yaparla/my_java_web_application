pipeline {
    agent any 
    tools {
        java 'JDK'
        maven 'maven'
    }
    stages {
        stage('Stage-1 : Clean') { 
            steps {
                sh 'mvn clean'
            }
        }
         stage('Stage-2 : Validate') { 
            steps {
                sh 'mvn validate'
            }
        }
         stage('Stage-3 : Compile') { 
            steps {
                sh 'mvn compile'
            }
        }
         stage('Stage-4 : Test') { 
            steps {
                sh 'mvn test'
            }
        }
	  stage('Stage-5 : Package') { 
            steps {
                sh 'mvn package'
            }
        }
	 stage('Stage-6 : Verify') { 
            steps {
                sh 'mvn verify'
            }
        }
          stage('Stage-7 : Install') { 
            steps {
                sh 'mvn install'
            }
        }   
    }
}
