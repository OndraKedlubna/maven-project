pipeline {
    agent any

    stages {
        stage('Priprava') {
             steps {
                 echo 'Zacinam se psychcicky pripravovat'
             }
        }


        stage('Build') {
            steps {
                echo 'Building..'
                bat 'mvn clean package'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
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