pipeline {
    agent any
    tools {
        maven 'Maven 3.6.3'
    }
    stages {
        stage ('Compile Stage') {

            steps {
                    echo 'maven compile'
                    sh 'mvn clean compile'
            }
        }

        stage ('Testing Stage') {

            steps {
                    echo 'maven test'
                    sh 'mvn test'
            }
        }


        stage ('Deployment Stage') {
            steps { 
                    echo 'maven deploy'
                    sh 'mvn deploy'
                }
            }
        }
    }
