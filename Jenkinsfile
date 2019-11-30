pipeline {
    agent any




    stages {
        stage('Priprava') {
             steps {
                 echo 'krok 1'
             }
             steps {
                 echo 'krok 2'
             }


        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}