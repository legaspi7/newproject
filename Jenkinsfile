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
        stage('Deploy prod') {
	when {
                branch 'production'
            }
	steps {
                echo 'Deploying production....'
            }
        }
        stage('Deploy master') {
	when {
                branch 'master'
            }
	steps {
                echo 'Deploying master....'
            }
    }
}
