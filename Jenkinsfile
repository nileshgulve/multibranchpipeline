
node('master') {
    // some block
	stage('continous download') {
		git 'https://github.com/nileshgulve/java-hello-world-with-maven.git'
	}
	stage('continous build') {
		sh 'mvn package'
	}
	stage ('continous Deployment')
	{	
		sh 'scp /home/ubuntu/.jenkins/workspace/scriptedpipeline/target/jb-hello-world-maven-0.2.0.jar ubuntu@172.31.43.52:/var/lib/tomcat9/webapps/qaenv.war'
	}
	stage('continous Testing') {
		sh 'echo "Testing Passed..."'
	}
	stage ('continous Delivery')
	{	
		sh 'scp /home/ubuntu/.jenkins/workspace/scriptedpipeline/target/jb-hello-world-maven-0.2.0.jar ubuntu@172.31.37.207:/var/lib/tomcat9/webapps/prodenv.war'
	}	
}
