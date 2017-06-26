pipeline{
	agent any

	stages{
		stage('build'){
			steps{
				sh 'whoami'
				sh 'echo $JAVA_HOME'
				sh 'which jar'
				sh 'ant -f build.xml -v'
			}
		}
	}
}