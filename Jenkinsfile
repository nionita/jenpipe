pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
		    echo "But the feature..."
		    pwd
		    ls -lah
		'''
            }
        }
    }
    post {
    	always {
	    echo 'This will always run'
	}
	success {
	    echo 'This is a successful run'
	}
	failure {
	    echo 'Oh! It is a bug...'
	}
    }
}
