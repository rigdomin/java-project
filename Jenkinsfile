pipeline{
	agent any

	options{
		buildDiscarder(LogRotator(numToKeepStr: '2', artifacteNumToKeepStr: '1'))
	}

	stages{
		stage('build'){
			steps{
				sh 'echo webhook'
				sh 'ant -f build.xml -v'
			}
		}
	}

	post{
		always{
			archiveArtifacts artifacts: 'dist/*.jar', fingerprint: true
		}
	}
}