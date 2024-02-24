
node('master') {
    // some block
	stage('continous download') {
		git 'https://github.com/nileshgulve/java-hello-world-with-maven.git'
	}
	stage('continous build') {
		sh 'mvn package'
	}
}
