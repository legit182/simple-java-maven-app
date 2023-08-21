node {
   docker.image('maven:3.9.3-eclipse-temurin-17-alpine').inside('-p 3000:3000') {
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
	stage('Test') {
		sh './jenkins/script/test.sh'
        }
    }
}
