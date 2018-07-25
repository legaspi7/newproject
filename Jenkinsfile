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
        stage('DeployDevelop') {
	when {
                branch 'develop'
            }
	steps {
                echo 'Deploying develop....'
            }
	}
    }
}
