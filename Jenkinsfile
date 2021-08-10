pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				sh 'echo "Changed and Building..."'
				sh 'chmod +x scripts/Linux-Build.sh'
				
				archiveArtifacts artifacts: 'bin/Debug/*', fingerprint: true
			}
		}
		stage('Test') {
			steps {
				sh 'echo "Running..."'
				sh 'chmod +x scripts/Linux-Run.sh'
				sh 'scripts/Linux-Run.sh'
			}
		}
	}
}

