pipeline {
    agent any

    stages {
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
	when {
                branch 'production'
            }
	steps {
                echo 'Deploying....'
            }
        }
    }
}
