pipeline{
    agent any

    stages('CI'){
        stage('checkout'){
            steps{
                echo 'Checkout'
                checkout scm

            }

        }
        stage('Build'){
            steps{
                echo'Checkout'
                sh 'mvn clean install'
            }
        }
        stage('Test'){
            steps{
                echo 'Test'
                sh 'mvn test'            }

        }
    }
}