pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo 'Hello'
            }
	}
        stage('Docker Build') {
            steps {
                sh '''
		cd azure-vote/
		docker images -a
		docker images -t jenkins-pipeline .
		docker images -a
		cd ..
		'''
            }
        }
    }
}
