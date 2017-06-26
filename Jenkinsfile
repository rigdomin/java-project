pipeline{
	agent any

	stages{
		stage('build'){
			steps{
				sh 'echo webhook'
				sh 'ant -f build.xml -v'
			}
		}
	}
}