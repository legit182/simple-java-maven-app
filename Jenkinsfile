node {
    stage('Build') {
        docker.image('maven:3.9.3-eclipse-temurin-17-alpine').inside {
            sh 'mvn --version'
        }
    }
    stage('Test') {
	docker.image('maven:3.9.3-eclipse-temurin-17-alpine').inside {
	    sh './jenkins/scripts/test.sh'
	}
    }
