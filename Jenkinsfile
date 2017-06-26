pipeline{
	agent any

	stages{
		stage('build'){
			steps{
				sh 'whoami'
				sh 'which java'
				sh 'which jar'
				sh 'echo ${JAVA_HOME}'
				sh 'ant -f build.xml -v'
			}
		}
	}
}