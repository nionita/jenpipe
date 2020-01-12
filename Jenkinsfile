pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh '''
		    echo "Multiline shell commands"
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
