
node('master') {
    // some block
	stage('continous download_loan') {
		git 'https://github.com/nileshgulve/java-hello-world-with-maven.git'
	}
	stage('continous build_loan') {
		sh 'mvn package'
	}
}
