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
}
