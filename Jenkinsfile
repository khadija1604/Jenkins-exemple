pipeline {
    agent any

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
