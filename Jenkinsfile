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
        stage('DeployProd') {
	when {
                branch 'production'
            }
	steps {
                echo 'Deploying production....'
            }
        }
        stage('DeployMaster') {
	when {
                branch 'master'
            }
	steps {
                echo 'Deploying master....'
            }
    }
}
